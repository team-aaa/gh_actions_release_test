source 'https://rubygems.org'

git_source(:github) { |repo_name| "https://github.com/#{repo_name}" }

# Specify your gem's dependencies in gh_actions_release_test.gemspec
gemspec

group :development, :test do
  gem 'rspec', '~> 3'
  gem 'ruby_standard', git: 'git@github.com:forward3d/ruby_standard.git', tag: 'v0.8.6'
end

group :test do
  gem 'rspec_junit_formatter', '~> 0.4', require: false
  gem 'simplecov', '~> 0.17', require: false
end
