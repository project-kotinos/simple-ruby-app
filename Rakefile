require 'bundler/setup'
require 'rspec/core/rake_task'
require 'yourbase/rspec/skipper'


Bundler::GemHelper.install_tasks


RSpec::Core::RakeTask.new :spec do |t|
  t.rspec_opts = ["-c", "-f progress", "-r ./spec/spec_helper.rb"]
  t.pattern = 'spec/**/*_spec.rb'
end

task :default => :spec
