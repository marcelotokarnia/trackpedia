# *TRACKPEDIA*

# 1. Setup Backend

### 1.1 Ruby 2.5.0

Install rbenv with `brew install rbenv`

Verify its installation with rbenv-doctor: `curl -fsSL https://github.com/rbenv/rbenv-installer/raw/master/bin/rbenv-doctor | bash`

You should see something like:

```
Checking for `rbenv' in PATH: /usr/local/bin/rbenv
Checking for rbenv shims in PATH: OK
Checking `rbenv install' support: /usr/local/bin/rbenv-install (ruby-build 20171226)
Counting installed Ruby versions: none
  There aren't any Ruby versions installed under `/Users/marcelotokarnia/.rbenv/versions'.
  You can install Ruby versions like so: rbenv install 2.2.4
Checking RubyGems settings: OK
Auditing installed plugins: OK
```

Install ruby 2.5.0 with `rbenv install 2.5.0` and verify its installation with `ruby -v`

### 1.2 sqlite3

Download its autoconf [HERE](https://www.sqlite.org/download.html)

`tar xvfz sqlite-autoconf-*.tar.gz`

`cd sqlite-autoconf-*`

`./configure --prefix = /usr/local`

`make`

`make install`

Verify its installation with `sqlite3 --version`

### 1.3 Rails

Install it with `gem install rails`

Verify it with `rails --version`

### 1.4 Gem Dependencies

Install them with `bundle install`

### 1.5 Create DB

`bin/rails db:migrate`

### 1.6 run server to port 3000

`bin/rails server`

# 2. Setup Frontend
