# TubesZB Home Assistant add-on repository

Addon-ons for Home Assistant that allow you to easily flash new firmware on your TubesZB Coordinators

[![Open your Home Assistant instance and show the add add-on repository dialog with a specific repository URL pre-filled.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Ftube0013%2Ftubeszb_addons)

## Add-ons provided by this repository

- **[TubesZB TI CC2652 FW Flasher](https://github.com/tube0013/tubeszb_addons/tree/main/tzb-cc2652-flasher/DOCS.md)**

    Flash FW to TubesZB TI CC2652 based Coordinators

- **[TubesZB Silicon Labs FW Flasher](https://github.com/tube0013/tubeszb_addons/blob/main/tzb-silabs-flasher/DOCS.md)**

    Flash FW to TubesZB SiliconLabs EFR32 based Coordinators

- **[TubesZB Zigpy-CLI Tools](https://github.com/tube0013/tubeszb_addons/blob/main/tzb-zigpy-cli-tools/DOCS.md)**

    Use the [Zigpy-CLI](https://github.com/zigpy/zigpy-cli) in an add-on!

## Installation

Click on the button below:

[![Open your Home Assistant instance and show the add add-on repository dialog with a specific repository URL pre-filled.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Ftube0013%2Ftubeszb_addons)

Or, in your Home Assistant, navigate to _Configuration_ > _Add-ons, Backups & Supervisor_ > _Add-on Store_ > _..._ > _Repositories_ and add `https://github.com/tube0013/tubeszb_addons` to the list.



![Supports aarch64 Architecture][aarch64-shield]
![Supports amd64 Architecture][amd64-shield]
![Supports armhf Architecture][armhf-shield]
![Supports armv7 Architecture][armv7-shield]
![Supports i386 Architecture][i386-shield]


[aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[armhf-shield]: https://img.shields.io/badge/armhf-yes-green.svg
[armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
[i386-shield]: https://img.shields.io/badge/i386-yes-green.svg


## Credits

The libraries that tools in this addons are based on:

- [beagleconnect / cc1352 flasher](https://git.beagleboard.org/beagleconnect/cc1352-flasher)
- [JelmerT / cc2538-bsl](https://github.com/JelmerT/cc2538-bsl)

Thanks to the following as well - **developers and contributors**:

- [@tmercenaruss](https://github.com/mercenaruss) for the updated cc1352-flasher using sockets for faster network flashing and other ideas!
- [@home-assistant](https://github.com/home-assistant) for the orginal Silicon Labs Flasher for which these addons were based.
