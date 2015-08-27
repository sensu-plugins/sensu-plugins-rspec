## Sensu-Plugins-rspec

[ ![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-rspec.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-rspec)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-rspec.svg)](http://badge.fury.io/rb/sensu-plugins-rspec)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-rspec/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-rspec)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-rspec/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-rspec)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-rspec.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-rspec)
[![Codeship Status for sensu-plugins/sensu-plugins-rspec](https://codeship.com/projects/9999a9c0-d266-0132-51a0-2e715b0dd4a0/status?branch=master)](https://codeship.com/projects/77533)

## Functionality

## Files
 * bin/check-rspec.rb

## Usage

Run entire suite of tests

`check-rspec -d /tmp/my_tests`

Run only one set of tests

`check-rspec -d /tmp/my_tests -s spec/test_one.rb`

Run tests with all options (except environment variables)

`check-rspec -b /usr/bin/ruby -i bin/rspec -d /tmp/my_tests -s spec`

Run tests with required options and multiple environment variables

`check-rspec -d /tmp/my_tests -e "aws_access_key_id=XX aws_secret_access_key=XX"``


## Installation

[Installation and Setup](http://sensu-plugins.io/docs/installation_instructions.html)

## Notes
