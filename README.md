# apotapenko.github.io

Hello! You're in the repository for website apotapenko.com

This document contains installation guide and commonly used commands.

For full tutorial refer to [tutorial](TUTORIAL.md) that explains some basics that you'll need to edit webpages and also gives some links for further reading.

# Installation

To render this website on Ubuntu 16.04 you need:

1. Install ruby-dev
```sh
# On Ubuntu
sudo apt-get install ruby-dev
# On OSX
brew install ruby
```

2. Install Jekyll gem
```sh
sudo gem install jekyll
```

3. Install tufte-jekyll requirements:
```sh
sudo gem install bundler
bundle install
bundle clean --force
```

4. Fire Jekyll to see the web page:
```sh
jekyll serve -w --port 7003
```

# Frequent commands

- Post the commited changes to the live website:
```sh
bundle exec rake publish
```
