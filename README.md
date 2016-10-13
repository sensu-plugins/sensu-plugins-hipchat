## Sensu-Plugins-hipchat

[ ![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-hipchat.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-hipchat)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-hipchat.svg)](http://badge.fury.io/rb/sensu-plugins-hipchat)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-hipchat/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-hipchat)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-hipchat/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-hipchat)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-hipchat.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-hipchat)

## Functionality

## Files
 * bin/handler-hipchat.rb

## Usage

```
{
  "hipchat": {
    "apikey": "1234abcdefg1234abcdefg",
    "apiversion": "v1",
    "room": "Ops",
    "from": "Sensu",
    "add_msg": "\"<br>command: #{@event['check']['command']}<br>occurrences: #{@event['occurrences']}\""
  }
}
```
## Installation

[Installation and Setup](http://sensu-plugins.io/docs/installation_instructions.html)

## Notes
