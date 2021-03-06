# KlickmailApi

Simple gem for Klickmail API wrapper

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'klickmail_api'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install klickmail_api

## Usage
Require the file in your class:
```ruby
require 'klickmail_api'
```

Use as follow:
```ruby
# To setup the Klickmail connection
connector = KlickmailApi::Connector.new
# To setup https
connector = KlickmailApi::Connector.new('https://www.klickmail.com.br/api')

connector.login(username: 'john', password: 'doe')
# The connector will return response message hash, if success the message will have sessid and session_name. Otherwise will return an error message.
```


## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/ignicaodigitalbr/klickmail_api. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in the KlickmailApi project’s codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/ignicaodigitalbr/klickmail_api/blob/master/CODE_OF_CONDUCT.md).
