# Everett

I'm an engineer and techno optimist interested in cloud infrastructure, databases, computer vision, and AI.

## Local development

GitHub Pages builds this site with the `github-pages` gem (Jekyll 3.9 / Liquid 4.0.3), which fails on Ruby 3.2+ (`undefined method 'tainted?'`). `.ruby-version` pins Ruby 3.1.2 for local builds:

```
rbenv install 3.1.2   # if needed
bundle install
bundle exec jekyll serve
```

`Gemfile.lock` only affects local builds; GitHub Pages uses its own pinned gem versions.
