# MySQL

You're like going to need a database. MySQL is popular. These instructions assume you've installed **Homebrew**.

## Installation

```shell
$ brew update
$ brew install mysql
```

(Optional) If you would like to make sure that MySQL doesn't get updated when you update Homebrew, do

```shell
$ brew pin mysql
```

## Setup

### Securing MySQL

After you install, MySQL is setup with no root password. It may not matter for your development environment. You would be able to login as root using

```shell
$ mysql -uroot
```

To secure your installation, though, run `mysql_secure_installation` and answer the prompts. It's a good idea to answer **Y** to get the most secure installation. Read the prompts to make sure you understand what's going on.

### Start and Stop

If you want MySQL to start at login, run

```shell
$ ln -sfv /usr/local/opt/mysql/*.plist ~/Library/LaunchAgents
```

Otherwise, you can start MySQL by running

```shell
$ mysql.server start
```

and stop by running

```shell
$ mysql.server stop
```

## SQL Client

If you don't want to use the MySQL command line client, you can install [MySQL Workbench](http://www.mysql.com/products/workbench).
