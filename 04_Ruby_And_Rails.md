# Ruby

## rbenv

Use [rbenv](https://github.com/rbenv/rbenv) to manage ruby installations. You may not ever need to manage more than one ruby installation. However, rbenv - similar to Homebrew - allows you to work without sudo and allows you to easily start over if you make mistakes.

Install with

```shell
$ brew install rbenv ruby-build
```

Add the following to your `.zshrc` file

```shell
#rbenv
eval "$(rbenv init -)"
```

and reload your shell.

## Install a Ruby

You'll need a Ruby to use with Rails. Once the Ruby is installed, we'll make it the global default, then install Bundler.

```shell
$ rbenv install 2.2.4
$ rbenv global 2.2.4
$ ruby -v
2.2.4
$ gem install bundler
$ rbenv rehash
```

# Rails

Install Rails, and you're ready to go

```shell
$ gem install rails
$ rbenv rehash
```
