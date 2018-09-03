# Change Log
This project adheres to [Semantic Versioning](http://semver.org/).

This CHANGELOG follows the format laid out [here](https://github.com/sensu-plugins/community/blob/master/HOW_WE_CHANGELOG.md)

## [Unreleased]

### Security
- updated `yard` dependency to `~> 0.9.11` per: https://nvd.nist.gov/vuln/detail/CVE-2017-17042 which closes attacks against a yard server loading arbitrary files (@majormoses)
- updated rubocop dependency to `~> 0.51.0` per: https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-8418 (@majormoses)

### Breaking Changes
- removed ruby support for `< 2.3` (@majormoses)

### Changed
- appeased the cops (@majormoses)
- bumped min `sensu-plugin` to the latest version of 2.x (@majormoses)
- update changelog guidelines location (@majormoses)

## [3.1.0] - 2018-09-03
### Added
- support list of hipchat rooms, so notifications are sent to multiple rooms (@cgarciaarano)

## [3.0.0] - 2017-12-07
### Breaking Changes
- bumped dependency of `sensu-plugin` to 2.x you can read about it [here](https://github.com/sensu-plugins/sensu-plugin/blob/master/CHANGELOG.md#v200---2017-03-29) (@multani)

### Fixed
- fix `timeout` runtime warnings (@multani)

## [2.1.0] - 2017-12-05
### Changed
- Remove trailing whitespace in the default template

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

[Unreleased]: https://github.com/sensu-plugins/sensu-plugins-hipchat/compare/3.1.0...HEAD
[3.1.0]: https://github.com/sensu-plugins/sensu-plugins-hipchat/compare/3.0.0...3.1.0
[3.0.0]: https://github.com/sensu-plugins/sensu-plugins-hipchat/compare/2.1.0...3.0.0
[2.1.0]: https://github.com/sensu-plugins/sensu-plugins-hipchat/compare/2.0.0...2.1.0
[2.0.0]: https://github.com/sensu-plugins/sensu-plugins-hipchat/compare/1.0.0...2.0.0
[1.0.0]: https://github.com/sensu-plugins/sensu-plugins-hipchat/compare/0.0.4...1.0.0
[0.0.4]: https://github.com/sensu-plugins/sensu-plugins-hipchat/compare/0.0.3...0.0.4
[0.0.3]: https://github.com/sensu-plugins/sensu-plugins-hipchat/compare/0.0.2...0.0.3
[0.0.2]: https://github.com/sensu-plugins/sensu-plugins-hipchat/compare/0.0.1...0.0.2
