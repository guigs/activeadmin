source "https://rubygems.org"

eval_gemfile(File.expand_path("Gemfile.common", __dir__))

group :release do
  gem 'chandler', '0.9.0' # Github releases from changelog
end

group :lint do
  # Code style
  gem 'rubocop', '0.75.0'
  gem 'rubocop-rspec', '~> 1.30'
  gem 'rubocop-rails', '~> 2.3'
  gem 'mdl', '0.5.0'

  # Translations
  gem 'i18n-tasks'
  gem 'i18n-spec'
end

group :docs do
  gem 'yard'     # Documentation generator
  gem 'kramdown' # Markdown implementation (for yard)
end

gem "rails", "~> 6.0.0"
gem "activerecord-jdbcsqlite3-adapter", "~> 60.0.rc1", platform: :jruby

gemspec path: "."
