# AocExecutor

Ruby executor for the [Advent of Code Solver](https://github.com/tcollier/aoc_solver).

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'aoc_executor'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install aoc_executor

## Usage

```ruby
# main.rb
require 'aoc_executor'

part1_proc = Proc.new { |input| compute_part1_solution(input) }
part2_proc = Proc.new { |input| compute_part2_solution(input) }
executor = AocExecutor.new(load_input, part1_proc, part2_proc)
executor.run(ARGV)
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/aoc_executor. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [code of conduct](https://github.com/[USERNAME]/aoc_executor/blob/master/CODE_OF_CONDUCT.md).

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in the AocExecutor project's codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/[USERNAME]/aoc_executor/blob/master/CODE_OF_CONDUCT.md).
