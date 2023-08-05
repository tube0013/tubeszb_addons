# TubesZB TI CC2652 Flasher Add-on

## Installation

Click on the button below:

[![Open your Home Assistant instance and show the add add-on repository dialog with a specific repository URL pre-filled.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Ftube0013%2Ftubeszb_addons)

Or, in your Home Assistant, navigate to _Configuration_ > _Add-ons, Backups & Supervisor_ > _Add-on Store_ > _..._ > _Repositories_ and add `https://github.com/tube0013/tubeszb_addons` to the list.

1. Navigate in your Home Assistant frontend to **Settings** -> **Add-ons, Backup & Supervisor** -> **Add-on Store**.
2. Find the "TubesZB TI CC2652 FW Flasher" add-on and click it.
3. Click on the "INSTALL" button.

## How to use

The add-on needs a TI CC2652 wireless module accessible through a network
serial port defined by IP addres and port or other USB based wireless adapters.

1. For a Network attached coordinator enter the IP_ADDRESS:port or 
   select the correct `device` in the add-on configuration tab and press `Save`.
2. Start the add-on.
3. Monitor the flash by goind to the addon log page, and refreshing periodically.

## Configuration

Add-on configuration:

| Configuration             | Description                                                      |
|---------------------------|------------------------------------------------------------------|
| device                    | Serial service where the Silicon Labs radio is attached          |
| network_device            | Network Serial port (IP_ADDRESS:PORT)                            |
| flow_control              | If hardware flow control should be enabled (depends on firmware) |
| firmware_url (mandatory)  | Custom URL to flash firmware from                                |

## Support

Got questions?

