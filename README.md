# CliQuestions

A ruby gem used for console applications. The Questions module conatins serveral functions that take a question and an array of possible responses.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'cli_questions'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install questions

## Usage

```ruby
irb(main):001:0> Questions.yes_or_no? "Do you like ruby?"
Do you like ruby?
1. Yes
2. No
1
=> true

irb(main):002:0> Questions.yes_or_no? "Can I pick something other then yes or no"
Can I pick something other then yes or no
1. Yes
2. No
3
Can I pick something other then yes or no
1. Yes
2. No
2
=> false

irb(main):003:0> Questions.pick_a_number "Which of these is a prime?", [ 6, 7, 8 ]
Which of these is a prime?
( 6, 7, 8 )
7
=> 7

irb(main):007:0> Questions.multichoice "Pick a color", ["green", "purple", "teal"]
Pick a color
1 : green
2 : purple
3 : teal
1
=> "green"

irb(main):008:0> Questions.multichoice "Pick a color", [:yellow, :red, :blue]
Pick a color
1 : yellow
2 : red
3 : blue
3
=> :blue
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/td-extreme/cli_questions. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [code of conduct](https://github.com/td-extreme/cli_questions/blob/master/CODE_OF_CONDUCT.md).


## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in the CliQuestions project's codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/[USERNAME]/cli_questions/blob/master/CODE_OF_CONDUCT.md).
