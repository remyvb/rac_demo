source 'https://rubygems.org'

group :development, :test do
  gem 'rake',    :require => false
  gem "puppet-blacksmith"
  platform :ruby_19, :ruby_20 do
    gem 'travis'
    gem 'travis-lint'
    gem 'ruby_gntp'
  end
end

group :test do
  gem 'puppet-lint',  :github => 'rodjek/puppet-lint'
  gem 'rspec-puppet', '~> 1.0.0'
  gem 'rspec-system-puppet'
  gem 'puppetlabs_spec_helper'
  gem 'puppet-syntax'
end

gem 'byebug'
if puppetversion = ENV['PUPPET_GEM_VERSION']
  gem 'puppet', puppetversion, :require => false
else
  gem 'puppet', :require => false
end
