source 'https://rubygems.org'

gem 'hashdiff'
gem 'rbvmomi'
gem 'net-ssh'
gem 'net-scp'

group :development, :test do
  gem 'rake', '<11.0'
  gem 'rspec', :require => false
  gem 'mocha', "~> 0.10.5", :require => false
  gem 'puppetlabs_spec_helper', :require => false
  gem 'puppet-lint', :require => false
  gem 'rspec-puppet', "2.4.0", :require => false
end

facterversion = ENV['GEM_FACTER_VERSION']
if facterversion
    gem 'facter', facterversion
else
    gem 'facter', '~> 2.0' :require => false
end

ENV['GEM_PUPPET_VERSION'] ||= ENV['PUPPET_GEM_VERSION']
if puppetversion = ENV['GEM_PUPPET_VERSION']
  gem 'puppet', puppetversion
else
  gem 'puppet', '5.3.3', :require => false
end
