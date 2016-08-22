source 'http://rubygems.org'

group :test do
  if puppetversion = ENV['PUPPET_GEM_VERSION']
    gem 'puppet', puppetversion, :require => false
  else
    gem 'puppet', ENV['PUPPET_VERSION'] || '~> 3.8.0'
  end

  gem 'rake'
  gem 'puppet-lint'
  gem 'rspec-puppet', :git => 'https://github.com/rodjek/rspec-puppet.git'
  gem 'puppet-syntax'
  gem 'puppetlabs_spec_helper'
  gem 'simplecov'
  gem 'metadata-json-lint'
  gem 'rspec-puppet-facts'

  gem "puppet-lint-absolute_classname-check"
  gem "puppet-lint-leading_zero-check"
  gem "puppet-lint-trailing_comma-check"
  gem "puppet-lint-version_comparison-check"
  gem "puppet-lint-classes_and_types_beginning_with_digits-check"
  gem "puppet-lint-unquoted_string-check"
  gem 'puppet-lint-resource_reference_syntax'
  gem 'rspec-puppet-facts'
end

group :development do
  gem 'puppet-blacksmith'
  gem 'guard-rake'
  gem 'listen', '<= 3.0.6'
end

group :system_tests do
  gem "beaker"
  gem "beaker-rspec"
  gem "beaker-puppet_install_helper", :require => false
end
