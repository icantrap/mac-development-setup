# Ruby And Maybe Rails

# rvm

[rvm](https://rvm.io) allows you to select between multiple installed versions of Ruby for your various projects.

```shell
$ gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3
$ \curl -sSL https://get.rvm.io | bash -s stable
```

After the installation is done, either close and reopen your console, or reload your shell resource file.

# Install a Ruby

Install a version of ruby like so:

```shell
$ rvm install 2.2.4
```

Make it your default ruby version:

```shell
$ rvm use 2.2.4 --default
```

To speed up your rubygem installations, you can make it so documentation doesn't get locally installed with the gem.

```shell
$ echo "gem: --no-ri --no-rdoc" > ~/.gemrc
```

# Rails

```shell
gem install rails
```

Pretty simple, right?
