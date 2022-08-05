# Change Log

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

## [Unreleased] - yyyy-mm-dd

## [0.1.0a4] - 2022-08-05

### Changed

- Remove support for Python 3.6
- Remove support for Django 3.1
- Add support for Django 3.2

### Fixed

- AA3 compatibility fix
- Handle AttributeError when deleting a User who doesn't have a main_character set

Thanks to @jtrenaud1s for the contribution!

## [0.1.0a3] - 2021-01-21

### Added

- Webhooks for alerting when:
  - Users hit inactivity thresholds
  - Leave of absence requests are created
  - Leave of absence requests are approved

## [0.1.0a2] - 2021-01-20

### Added

- Provide a way to view request notes from the frontend
- New datepicker on LOA request creation

### Changed

- Made request approval status more accessible (and added colors)

### Fixed

- CSS for buttons to approve requests

## [0.1.0a1] - 2021-01-17

### Added

- Initial Release
