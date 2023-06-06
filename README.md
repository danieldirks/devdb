# devdb

Fire up a local testing database from a dump in no time.

[![MIT License](https://img.shields.io/github/license/danieldirks/devdb.svg)](LICENSE)


## Features

* Easy setup of local dev databases without the hassle.
* Loads a dump on startup, so you don't have to worry how to get your data in.
* Supports MySQL, MariaDB and PostgreSQL.
* Uses docker to start temporary databases without cluttering up your device.
* Lets you export to share, customize and set up on other machines.


## Setup

Make sure docker is installed and run `curl -sSf https://raw.githubusercontent.com/danieldirks/devdb/main/devdb > ~/.local/bin/devdb`.

To update or uninstall, simply remove the file and load it again.


## Usage

1. `devdb dump.sql`
2. wait
3. connect

It tries its best to figure out the database management system for you by searching for one of the supported databases at the beginning of the dump file. In some cases you may still need to specify it manually: `devdb --base mysql dump.sql`.

You can customize things like user and password and can export `devdb`s. More can be found by running `devdb help`.

Save time and have fun!


## License

The project is licensed under the [MIT License](LICENSE).
