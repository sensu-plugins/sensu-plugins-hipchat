# Change Log
This project adheres to [Semantic Versioning](http://semver.org/).

This CHANGELOG follows the format listed at [Keep A Changelog](http://keepachangelog.com/)

## [Unreleased]
### Changed
- updated sensu-plugin gem to `~> 2.0`
- fix runtime warnings

## [2.0.0] - 2017-07-24
### Breaking Changes
- Minimum Ruby runtime version is now 2.0

## [1.0.0] - 2017-07-12
### Added
- Ruby 2.4.1 testing

### Breaking Changes
- Dropped Ruby 1.9.3 support

### Changed
- added option to configure message format in ERB template
- added option to configure message format as either `html`(default) or `text`

## [0.0.4] - 2016-08-10
### Changed
- Updated sensu-plugin dependency from `= 1.2.0` to `~> 1.2`
- improved description for --json_config option

## [0.0.3] - 2015-07-14
### Changed
- updated sensu-plugin gem to 1.2.0

### Added
- ability to specify the room at the check level

## [0.0.2] - 2015-06-02
### Fixed
- added binstubs
### Changed
- removed cruft from /lib

## 0.0.1 - 2015-05-29
### Added
- initial release

[Unreleased]: https://github.com/sensu-plugins/sensu-plugins-hipchat/compare/2.0.0...HEAD
[2.0.0]: https://github.com/sensu-plugins/sensu-plugins-hipchat/compare/1.0.0...2.0.0
[1.0.0]: https://github.com/sensu-plugins/sensu-plugins-hipchat/compare/0.0.4...1.0.0
[0.0.4]: https://github.com/sensu-plugins/sensu-plugins-hipchat/compare/0.0.3...0.0.4
[0.0.3]: https://github.com/sensu-plugins/sensu-plugins-hipchat/compare/0.0.2...0.0.3
[0.0.2]: https://github.com/sensu-plugins/sensu-plugins-hipchat/compare/0.0.1...0.0.2
