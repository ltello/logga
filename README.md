# Logga

Welcome to your new gem! In this directory, you'll find the files you need to be able to package up your Ruby library into a gem. Put your Ruby code in the file `lib/logga`. To experiment with that code, run `bin/console` for an interactive prompt.

TODO: Delete this and the text above, and describe your gem

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'logga'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install logga

## Usage

Add this to your model:

```ruby
class Order < ApplicationRecord
  add_log_entries_for :create, :update
end

```

so that new LogEntry records attached to a given Order instance will be created whenever a new one is created or
modified.

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then `git push gemfury master` where gemfury remote is `https://[YOUR GEM FURY USER NAME]git.fury.io/boxt/logga_engine.git`.

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/ltello/logga.

## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
