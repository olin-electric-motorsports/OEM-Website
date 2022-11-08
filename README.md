# OEM Website

This website is built with [Jekyll](https://jekyllrb.com/docs/).

# Ubuntu Setup

To view changes locally on Ubuntu, you need to install Ruby and Jekyll.

These instructions install an outdated version, but it's what the getting started suggests and seems to work.

1. Remove existing installation

    ```
    sudo apt-get remove ruby
    sudo apt update
    ```
1. Install dependencies
    ```
    sudo apt install git curl libssl-dev libreadline-dev zlib1g-dev autoconf bison build-essential libyaml-dev libreadline-dev libncurses5-dev libffi-dev libgdbm-dev -y
    ```
1. Install Ruby
    ```
    curl -sL https://github.com/rbenv/rbenv-installer/raw/main/bin/rbenv-installer | bash -
    ```
1. Run this command and follow the directions to set up for your shell.
    ```
     ~/.rbenv/bin/rbenv init
    ```
1. Install Ruby 2.5.4
    ```
    rbenv install 2.5.4
    rbenv global 2.5.4
    ```
1. Install Jekyll and bundler
    ```
    gem install jekyll bundler
    ```
1. CD into the cloned repository and install dependencies
    ```
    cd /path/to/repo
    bundle install
    ```
1. Build the website
    ```
    bundle exec jekyll serve
    ```
