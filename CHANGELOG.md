# Changelog

## [1.0.4] - 2026-01-12

### Fixed
- Notification click actions now open the HA app directly instead of browser (uses `homeassistant://navigate/` scheme)

## [1.0.3] - 2026-01-12

### Changed
- Replaced `gcode_filename` input with `task_name` for proper print job names
- Now uses `end_time` entity for finish time instead of calculating from remaining time

## [1.0.2] - 2026-01-12

### Fixed
- Fixed filament runout detection - now correctly monitors `paused_filament_runout` state

### Added
- AMS connection lost detection (`paused_ams_lost`)
- Nozzle clog detection (`paused_nozzle_clog`)
- Dynamic alert messages based on issue type

## [1.0.1] - 2026-01-11

### Added
- Estimated finish time displayed in notifications (e.g., "done ~3:45 PM")

## [1.0.0] - 2026-01-11

### Added
- Initial release
- Print start, completion, and failure notifications
- Progress notifications at 25%, 50%, 75%, 100%
- Persistent notification with live progress bar
- Camera snapshot support in notifications
- Filament runout detection
- Pause/resume notifications
- Printer offline detection (5-minute delay to avoid false positives)
- AMS device monitoring support (up to 4 AMS units + AMS HT)
- Quiet hours configuration
- Dual-nozzle printer support (active nozzle + individual nozzle 1/2 temps)
- Customizable notification service
- Deep links to printer dashboard
- Anti-spam protections to prevent duplicate notifications
