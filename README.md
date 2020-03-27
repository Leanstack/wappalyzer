# Wappalyzer

  This is merely a port of the javascript parts of Wappalyzer extension for Firefox and Chrome. It analyzes a url and tries to guess what software it uses (like server software, CMS, framework, programming language).

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'wappalyzer'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install wappalyzer

# Usage

```
url = "https://www.heroku.com/"
Wappalyzer::Detector.new.analyze(url)
```

## Output

```
{
  "Cowboy" => {
    "categories" => [
      [0] "web-frameworks",
      [1] "web-servers"
    ],
    "confidence" => 100,
    "version" => ""
  },
  "Google Tag Manager" => {
    "categories" => [
      [0] "tag-managers"
    ],
    "confidence" => 100,
      "version" => ""
  },
  "Ruby on Rails" => {
    "categories" => [
      [0] "web-frameworks"
    ],
    "confidence" => 50,
    "version" => ""
  },
  "Erlang" => {
    "categories" => [
      [0] "programming-languages"
    ],
    "confidence" => 100,
      "version" => ""
  },
  "Ruby" => {
    "categories" => [
      [0] "programming-languages"
    ],
    "confidence" => 50,
      "version" => ""
  }
}
``` 




## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/pulkit21/wappalyzer. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

