# Execute bundler hook if present
['~/.', '/etc/'].any? do |file|
 File.lstat(path = File.expand_path(file + 'bundle-gemfile-hook')) rescue next
 eval(File.read(path), binding, path); break true
end || source('https://rubygems.org/')

gem 'chalk-hostname', :git => 'git@github.com:stripe/chalk-hostname', :ref => 'c362f40046d2a1188bca11c969611a4bca1b9c37'
gem 'space-commander', :git => 'git@github.com:stripe-internal/space-commander', :ref => 'd1d7da58aa7972b124b090204b7e94be19fe0756'

# Specify your gem's dependencies in yoyo.gemspec
gemspec
