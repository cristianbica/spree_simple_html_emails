Spree Simple HTML Emails
=====================

Sends easily configurable, scss powered, localised html multipart emails from spree. Insired by spree-html-email, but brought up to date with spree 2-1-stable.

* Automatically includes your site logo
* Set your site colours just by editing a few SCSS variables
* Sets links back to your site automatically
* Fully localised

All emails are direct copies of spree's emails with some light HTML formatting, and the original `content.text.erb` from spree is still sent as a multi part for none HTML clients.

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