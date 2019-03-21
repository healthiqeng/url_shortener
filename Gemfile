source 'https://rubygems.org'

git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby "2.5.0"

# Configs common to all environments
gem 'rails', '~> 5.0.6'             # Ruby on rails
gem 'custom_configuration'          # allows config.x.whatever
gem 'multi_json', '~> 1.2'
gem 'pg'                            # postgresql database
gem 'puma', '~> 3.0'                # Use puma as the app web server
gem 'rack-attack'                   # Security, performance

gem 'jquery-rails'                  # Build JSON APIs
gem 'delayed_job_active_record'

group :development do
  gem 'annotate'
  gem 'web-console', '>= 3.3.0'
  gem 'listen', '~> 3.0.5'
  gem 'byebug', platform: :mri
  gem 'rb-readline'
end

group :development, :test do
  gem 'figaro'
  gem 'rspec-rails', '~> 3.8'
  gem 'rubocop', '~> 0.53.0', require: false
  gem 'spring'
  gem 'spring-watcher-listen', '~> 2.0.0'
end

group :test do
  gem 'database_cleaner'
  gem 'factory_bot_rails'
  gem 'simplecov'
end

group :staging, :production do
end
