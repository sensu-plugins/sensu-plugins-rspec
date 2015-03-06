## Sensu-Plugins-rspec

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-rspec.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-rspec)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-rspec.svg)](http://badge.fury.io/rb/sensu-plugins-rspec)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-rspec/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-rspec)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-rspec/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-rspec)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-rspec.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-rspec)

## Functionality

## Files
 * bin/check-rspec

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

Add the public key (if you haven’t already) as a trusted certificate

```
gem cert --add <(curl -Ls https://raw.githubusercontent.com/sensu-plugins/sensu-plugins.github.io/master/certs/sensu-plugins.pem)
gem install sensu-plugins-rspec -P MediumSecurity
```

You can also download the key from /certs/ within each repository.

#### Rubygems

`gem install sensu-plugins-rspec`

#### Bundler

Add *sensu-plugins-disk-checks* to your Gemfile and run `bundle install` or `bundle update`

#### Chef

Using the Sensu **sensu_gem** LWRP
```
sensu_gem 'sensu-plugins-rspec' do
  options('--prerelease')
  version '0.0.1'
end
```

Using the Chef **gem_package** resource
```
gem_package 'sensu-plugins-rspec' do
  options('--prerelease')
  version '0.0.1'
end
```

## Notes
