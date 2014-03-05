source ENV['GEM_SOURCE'] || 'https://rubygems.org'

if puppetversion = ENV['PUPPET_VERSION']
	  gem 'puppet', puppetversion, :require => false
else
	  gem 'puppet', :require => false
end

gem 'rspec_junit_formatter'
gem 'puppet-lint'
gem 'rspec-puppet', :git => 'https://github.com/rodjek/rspec-puppet.git'
gem 'puppetlabs_spec_helper', '>= 0.1.0'

group :systemtests do
  gem 'beaker'
  gem 'beaker-rspec'
  gem 'pry'
end
