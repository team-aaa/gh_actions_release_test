namespace :bundler do
  require 'bundler/gem_tasks'
end
require 'rspec/core/rake_task'

RSpec::Core::RakeTask.new(:spec)

task default: :spec
desc "Wrap Bundler's release task with BUNDLE_GEM__PUSH_KEY setting"
task :release do
  Bundler.settings.set_local('gem.push_key', 'github')
  Rake::Task['bundler:release'].invoke
end
