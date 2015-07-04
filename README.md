[![Gem Version](https://badge.fury.io/rb/binlist.svg)](http://badge.fury.io/rb/binlist) [![Inline docs](http://inch-ci.org/github/CodeHaven9ja/binlist.svg?branch=master)](http://inch-ci.org/github/CodeHaven9ja/binlist)
# Binlist

Binlist is a simple gem for searching Issuer Identification Numbers (IIN). The first 6 digits of a credit card number are known as the Issuer Identification Number (IIN), previously known as Bank Identification Number (BIN). These identify the institution that issued the card to the card holder. 

This gem queries [Binlist.net](http://Binlist.net) public REST api.

### Limits
Due to the high volume of queries [Binlist.net](http://Binlist.net) has implemented a throttling mechanism, which allows at most 10,000 queries per hour. After reaching this hourly quota, all your requests result in HTTP 403 (Forbidden) until it clears up on the next roll over. 

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'binlist'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install binlist

## Usage

Binlist.find(######)

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release` to create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

1. Fork it ( https://github.com/CodeHaven9ja/binlist/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
