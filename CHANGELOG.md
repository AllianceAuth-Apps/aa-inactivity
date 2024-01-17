# Change Log

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

## [Unreleased] - yyyy-mm-dd

## [1.1.0] - 2024-01-17

### Changed

- Added support for AA4
- Add missing docstrings
- Add pylint checks

## [1.0.0] - 2023-07-18

### Added

- Adds a menu to the UI
- Show badge for unapproved requests in side bar
- Handling for HTTP 429 errors
- Auto retry on network timeouts
- Add tab to show all approved requests
- Page showing currently inactive users

### Changed

- When creating InactivityPing objects set timestamp via Django default factory
- Switch to py-cord library for sending to Discord webhooks due to built in handling of rate limits
- Check inactivity for users in parallel
- Run tasks with slightly lower default priority to avoid congestion
- Drops support for Python 3.7
- Adds support for Python 3.10
- Moved build process to PEP 621
- Drops support for AA2
- Adds support for AA3
- Adds support for Python 3.11
- Breaking change: Dropped support for aa_discordbot. Notifications are generated to Auth. You can install Discord Notify to get them on Discord like before.
- Show users with character icon in lists
- Approver needs to provide reason for rejecting loa requests
- Denied requests are kept and shown in requests history

### Fixed

- Can create requests with overlapping time frames

## [0.1.0a7] - 2023-05-21

### Fixed

- Can only create new requests when running in English locale

## [0.1.0a6] - 2022-08-06

### Changed

- Exclude incompatible Member Audit versions in requirements

## [0.1.0a5] - 2022-08-06

### Changed

- Adopt new MemberAudit API for compatibility with upcoming model change

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
