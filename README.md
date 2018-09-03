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
    "message_template": "optional message template erb file path - /some/path/to/template.erb",
    "message_format": "html"
  }
}
```
## Installation

[Installation and Setup](http://sensu-plugins.io/docs/installation_instructions.html)

## Notes

### message_template example

```
<%=
[
  @event["action"].eql?("resolve") ? "RESOLVED" : "ALERT",
  " - [#{event_name}]<br>",
  "command: #{@event['check']['command']}<br>",
  "occurrences: #{@event['occurrences']}<br>",
  @event["check"]["notification"] || @event["check"]["output"],
  "<br>",
  playbook,
].join
%>
```

### How to test?

1. Write a configuration file as explained in the *Usage* section
1. Set the environment variable `SENSU_CONFIG_FILES` to the location of this file
1. Pipe a sample check result into the handler itself:
```
cat <<EOF | bundle exec bin/handler-hipchat.rb
{
  "client": {
    "name": "client"
  },
  "check": {
    "status": 1,
    "name": "name",
    "source": "source",
    "output": "Hello, warning",
    "hipchat_room": ["general","important"]
  }
}
EOF
```
