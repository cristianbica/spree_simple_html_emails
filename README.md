Spree Simple HTML Emails
=====================

Wraps Sprees default text.erb emails in a html wrapper, then parses the original text files rather than using extra templates

Installation
------------

Add spree_simple_html_emails to your `Gemfile`:

```ruby
gem 'spree_simple_html_emails', git: 'https://github.com/200Creative/spree_simple_html_emails', branch: 'master'
```

This uses premailer to inline CSS styles. premailer-rails requires either [nokogiri] or [hpricot]. It doesn't list them as
a dependency so you can choose which one to use. Since hpricot is no longer
maintained, I suggest you to go with nokogiri. Add either one to your `Gemfile`:

```ruby
gem 'nokogiri'
# or
gem 'hpricot'
```

If both gems are loaded for some reason, premailer chooses hpricot.