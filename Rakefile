require "bundler/setup"
require "bundler/gem_tasks"
require "rspec/core/rake_task"

namespace :spec do
  RSpec::Core::RakeTask.new(unit: :build) do |task|
    task.pattern = FileList['spec/**/*_spec.rb']
  end
end

task default: 'spec:unit'
