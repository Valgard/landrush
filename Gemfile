source 'https://rubygems.org'

# Can't use `gemspec` to pull in dependencies, because the landrush gem needs
# to be in the :plugins group for Vagrant to detect and load it in development

gemspec

# Vagrant's special group
group :plugins do
  gem 'landrush', path: '.'
end

group :development do
  gem 'vagrant',
      :git => 'git://github.com/mitchellh/vagrant.git',
      :ref => 'v1.8.4'

  gem 'rake', '~> 10'
  gem 'rubocop', '~> 0.38.0'
  gem 'byebug'
  gem 'mocha'
  gem 'minitest'
  gem 'cucumber', '~> 2.1'
  gem 'aruba', '~> 0.13'
  gem 'komenda', '~> 0.1.6'
end
