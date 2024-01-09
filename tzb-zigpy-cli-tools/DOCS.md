# TubesZB Add-on: Zigpy-CLI Tools Add-on

## Installation

Click on the button below:

[![Open your Home Assistant instance and show the add add-on repository dialog with a specific repository URL pre-filled.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Ftube0013%2Ftubeszb_addons)

Or, in your Home Assistant, navigate to _Configuration_ > _Add-ons, Backups & Supervisor_ > _Add-on Store_ > _..._ > _Repositories_ and add `https://github.com/tube0013/tubeszb_addons` to the list.

1. Navigate in your Home Assistant frontend to **Settings** -> **Add-ons, Backup & Supervisor** -> **Add-on Store**.
2. Find the "TubesZB Zigpy-CLI Tools" add-on and click it.
3. Click on the "INSTALL" button.

## How to use

*Disable/Stop ZHA or Zigbee2MQTT when using this addon*

# Select yor coordinator's path
Pick the serial port for your USB connected Coordinator, or Select USE Network Device and enter the IP address and Port (IP_ADDRESS:PORT) of the coordinator

# Pick Radio Type and Baudrate
Pick your radio type from the drop down. 
| Radio Type | Description                                                     |
|------------|-----------------------------------------------------------------|
| znp        | Texas Instruments Z-Stack ZNP protocol: CC253x, CC26x2, CC13x2  |
| ezsp       | Silicon Labs EmberZNet protocol: Elelabs, HUSBZB-1, Telegesis   |
| deconz     | dresden elektronik deCONZ protocol: ConBee I/II, RaspBee I/II   |
| xbee       | Digi XBee Zigbee radios: Digi XBee Series 2, 2C, 3              |
| zigate     | ZiGate Zigbee radios: PiZiGate, ZiGate USB-TTL, ZiGate WiFi     |
| zboss      | Nordic Semiconductor nRF modules                                |

*Note some radios do not work with all the tools xbee for example*

Pick the Baudrate for your radio, if you don't know it leave it at 115200

# Pick the Zigpy-CLI command to use
Currently 4 commands are supported from zipy-cli
* **Info** - Read the network information from the radio
* **Energy Scan** -  Perform an energy scan
* **Form** - Form a network on a new coordinator
* **Reset** - Resets the radio removing its network configuration

# Start the addon
Start the Addon from the Info Tab.
Switch over the the Log Tab to see the tools output, refresh the log occasionally to get the lasted updates of the console/command output.
When done, be sure the addon is stopped before restarting ZHA or Zigbee2MQTT

## Configuration

Add-on configuration:

| Configuration      | Description                                            |
|--------------------|--------------------------------------------------------|
| device             | Serial service where the radio is attached |
| network_device     | Network Serial port (IP_ADDRESS:PORT)
| radio_type         | Type of radio / coordinator
| baudrate           | Serial port baudrate (depends on firmware)   |
| action             | zigpy-cli command to run |


