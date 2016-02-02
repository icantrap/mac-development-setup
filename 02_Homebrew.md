# Homebrew

[Homebrew](http://brew.sh) is a package manager for OS X. There are many advantages to using Homebrew. If you're familiar with other package managers, you wont have much problem with Homebrew. Documentation is [here](https://github.com/Homebrew/homebrew/tree/master/share/doc/homebrew#readme).

## XCode Command Line Tools

You need XCode Command Line Tools to install Homebrew.

XCode is a huge download (over 4GB). However, unless you're using XCode for something like iPhone app development, you don't need to download it. You can simply download the Command Line Tools separately.

```shell
$ xcode-select --install
```

When it asks for your password, provide it.

## Installation

Installing Homebrew is done on the command line. From the Homebrew website:

```shell
$ `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
```

Homebrew is not run as root. Do not preprend `sudo` to the command.

Just for kicks, lets install a couple of useful packages:

```shell
$ brew install git
$ brew install ack
```

I install git to replace the outdated version provided by OS X. [ack](http://beyondgrep.com) is a `grep` replacement written with source code in mind.
