# encoding: utf-8

require 'rubygems'
require 'bundler'
begin
  Bundler.setup(:default, :development)
rescue Bundler::BundlerError => e
  $stderr.puts e.message
  $stderr.puts "Run `bundle install` to install missing gems"
  exit e.status_code
end
require 'rake'

require 'jeweler'
Jeweler::Tasks.new do |gem|
  # gem is a Gem::Specification... see http://docs.rubygems.org/read/chapter/20 for more options
  gem.name = "banorte_payworks"
  gem.homepage = "http://github.com/netmask/banorte_payworks"
  gem.license = "MIT"
  gem.summary = %Q{Simple TPV for Banorte Payworks Mexican Gateway}
  gem.description = %Q{}
  gem.email = "jonathan@devmask.net"
  gem.authors = ["Jonathan Garay"]
  # dependencies defined in Gemfile
end
Jeweler::RubygemsDotOrgTasks.new

require 'rspec/core'
require 'rspec/core/rake_task'
RSpec::Core::RakeTask.new(:spec) do |spec|
  spec.pattern = FileList['spec/**/*_spec.rb']
  # spec.version = "0.1.0"
end

task :default => :spec

require 'yard'
YARD::Rake::YardocTask.new
