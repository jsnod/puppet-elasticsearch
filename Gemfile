source ENV['GEM_SOURCE'] || 'https://rubygems.org'

if puppetversion = ENV['PUPPET_VERSION']
	  gem 'puppet', puppetversion, :require => false
else
	  gem 'puppet', :require => false
end

group :rspec do
  gem 'puppet-lint'
  gem 'rspec-puppet', :git => 'https://github.com/rodjek/rspec-puppet.git'
  gem 'puppetlabs_spec_helper', '>= 0.1.0'
  gem 'rspec_junit_formatter'
end

group :systemtests do
  gem 'beaker'
  gem 'beaker-rspec'
  gem 'pry'
  gem 'rspec_junit_formatter'
end

group :doclint do
  gem 'puppet-doc-lint', :git => 'https://github.com/petems/puppet-doc-lint.git'
end
