capistrano-copy-files
=====================

Capistrano v3.* extension for copying files between releases

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'capistrano', '~> 3.3.0'
gem 'capistrano-copy-files'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install capistrano-copy-files

## Usage

Require in `Capfile` to use the default task:

```ruby
require 'capistrano/copy_files'
```

The task will run during `deploy:updating` as part of Capistrano's default deploy

Configurable options:

```ruby
set :copy_files, []                       # default
set :copy_file_flags, ""                  # default
set :copy_dir_flags, "-R"                 # default
```
