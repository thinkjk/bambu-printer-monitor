# Bambu Lab 3D Printer Monitor

A Home Assistant Blueprint for monitoring Bambu Lab 3D printers with smart notifications.

## Features

- Print start, completion, and failure notifications
- Progress updates at 25%, 50%, 75%, and 100%
- Persistent notification with live progress bar
- Camera snapshots in notifications
- Filament runout detection
- Pause/resume notifications
- Printer offline alerts
- AMS filament monitoring support
- Quiet hours configuration
- Dual-nozzle printer support

## Requirements

- Home Assistant
- [Bambu Lab integration](https://github.com/greghesp/ha-bambulab)
- Mobile app for notifications (optional)

## Installation

1. Click the button below to import the blueprint:

   [![Open your Home Assistant instance and show the blueprint import dialog with this blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://github.com/thinkjk/bambu-printer-monitor/blob/main/bambu_printer_monitor.yaml)

2. Or manually copy `bambu_printer_monitor.yaml` to your `config/blueprints/automation/` directory

3. Create a new automation from the blueprint and configure your printer entities

## Configuration

| Option | Description |
|--------|-------------|
| Printer Name | Custom name for notifications |
| Print Status Entity | Main status sensor from Bambu Lab integration |
| Print Progress Entity | Progress percentage sensor |
| Current Stage Entity | Current printing stage sensor |
| Temperature Entities | Bed and nozzle temperature sensors |
| Nozzle 1/2 Temperature | Optional - individual nozzle temps for dual-extruder printers |
| Camera Entity | Printer camera for snapshots |
| Notify Device | Mobile device for notifications |
| AMS 1-4 | Optional - up to 4 AMS units for filament monitoring |
| AMS HT | Optional - AMS HT for high-temperature filaments |
| Progress Updates | Enable 25/50/75/100% notifications |
| Persistent Notification | Show live updating progress bar |
| Quiet Hours | Suppress non-critical notifications |

## License

MIT
