# This Gemfile installs dependencies for locally rendering the files in docs/
source 'https://rubygems.org'

gem 'jekyll-seo-tag'
gem 'jekyll-remote-theme'
gem 'jekyll-github-metadata'
gem 'webrick'

# The following plugins are enabled on GitHub Pages without a _config.yml.
gem 'jekyll-optional-front-matter'
gem 'jekyll-readme-index'
gem 'jekyll-relative-links'
gem 'jekyll-default-layout'
gem 'kramdown-parser-gfm'

# Replacing deprecated gems
gem 'csv'
gem 'json', '>= 2.10.2'

# GitHub Pages doesn't support jekyll 4.0 yet
gem 'jekyll', '<4.0'

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]

# Performance-booster for watching directories on Windows
gem 'wdm', '~> 0.1.0' if Gem.win_platform?
