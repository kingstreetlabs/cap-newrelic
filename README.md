# Cap::NewRelic

New Relic Deployment API support for Capistrano 3.x

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'capistrano', '~> 3.1.0'
gem 'cap-newrelic'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install cap-newrelic

## Usage

Require the module in your `Capfile`:

```ruby
require 'capistrano/newrelic'
```

`cap-newrelic` comes with 1 task `newrelic:notify`.

By default the task will run after `deploy:finished`


### Configuration

Configurable options, shown here with defaults:

```ruby
set :new_relic_api_key, nil
set :new_relic_url, nil
```

`new_relic_api_key` is required.
If not present `new_relic_api_key` will in `ENV['NEW_RELIC_API_KEY']`.

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request


## Thanks

This code started out based on [https://github.com/gunnarlium/capistrano-new-relic](https://github.com/gunnarlium/capistrano-new-relic) (for Capistrano v2)
