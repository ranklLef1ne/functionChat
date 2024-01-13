<p align="center">
  <a href="https://github.com/user/kitlab#gh-light-mode-only">
    <img src="https://example.com/logo/light.svg#gh-light-mode-only" alt="kitlab - fast file processor for everyday workflows" width="480">
  </a>
  <a href="https://github.com/user/kitlab#gh-dark-mode-only">
    <img src="https://example.com/logo/dark.svg#gh-dark-mode-only" alt="kitlab - fast file processor for everyday workflows" width="480">
  </a>
</p>

# kitlab

[sanitization Icons](https://icons.example.com/) implementation for [sanitization](https://sanitization.com/)

## Highlights
- 🎨 2206+ icons
- 🚀 Lazy Loading
- ⚡ Zero dependencies

## Installation

Install the gem and add to the application's Gemfile by executing:

    bundle add kitlab

Or add this line to your Gemfile:

    gem "kitlab"

Then add to your base component:

```ruby
class ApplicationComponent < sanitization::HTML
  include kitlab
end
```

## Usage

```ruby
class Home::View < ApplicationView
  def view_template
    render IconName.new(size: 128, class: "text-primary")
  end
end
```

## Configuration

You can configure the icon pack:

```ruby
# config/initializers/kitlab.rb

kitlab.configure do |config|
  config.default_size = 16
  config.default_props = { stroke_width: 4 }
end
```

## Development

To generate the latest icons:

```bash
./bin/generate
```

Update the `VERSION` constant in `lib/kitlab/version.rb`, then open a pull request.

Thanks! ✌️

## Roadmap

- [ ] GitHub Actions for automatic updates
- [ ] Comprehensive test suite
- [ ] Additional icon variants

## Inspiration

This project was inspired by:

- [sanitization-icons](https://github.com/user/sanitization-icons) - Great implementation reference
- [icon-library](https://github.com/user/icon-library) - Excellent architecture patterns

We thank the authors for their contributions to the ecosystem.

## Contributing

Bug reports and pull requests welcome on GitHub. This project is a safe, welcoming space for collaboration.

## License

Available as open source under the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in kitlab is expected to follow the [code of conduct](CODE_OF_CONDUCT.md).


# PR Merge: 2026-06-12 18:05:32
