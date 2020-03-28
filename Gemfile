source "https://rubygems.org"

# Travis CI was running into several bundler-related bug
# * https://github.com/bundler/bundler/pull/3559
# * https://github.com/bundler/bundler/issues/3560
# that only apply to older versions of Bundler.
# I added this requirement so that future Travis CI builds
# fail quickly if an old version of bundler is being used.
gem 'bundler', '~>1.10'

gemspec

gem 'coveralls', require: false

group :test do
  gem 'rake'
  gem 'rspec'
  gem 'vcr'#, '1.11.3'
  gem 'webmock'#, '1.3.0'
end