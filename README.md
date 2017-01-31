# LibreTaxi, open source alternative for Uber/Lyft

LibreTaxi makes taxis affordable again by completely removing all layers in between. Passengers pay with cash and get connected with drivers directly, where LibreTaxi is a thin layer allowing to negotiate the price before order is confirmed. No registration/approval is required. Less regulations.

Available at [@libretaxi_bot](https://telegram.me/libretaxi_bot).

## Implementation details

Technical stack:

* Node.js, JavaScript (ES6)
* Firebase as data storage
* Redis as storage for [kue](https://github.com/Automattic/kue)
* [Telegram](https://telegram.org) as the main transport
* CLI as backup and PoC transport

Translatable via locale file. Currently has support of the following languages:

* English
* Spanish
* Portuguese
* Indonesian (app only, [help us translating the website](https://github.com/ro31337/libretaxi-www/issues/3))
* Russian
* (on the way) Persian [help us translating to Persian](https://github.com/ro31337/libretaxi/issues/424)

Server support: macOS and Linux.

Client (Telegram) support: iOS, Android, macOS desktop client, web (can also work for Windows phones - not tested). Note that Telegram desktop clients for Linux and Windows are currently not supported because of lack location functionality. However, web client can be used on these OS along with any modern browser.

## Why Telegram?

* Available for all popular platforms
* Contains rich bot API
* Fast, reliable, and secure
* Works perfect with slow/poor Internet connection
* Staff and support are developer-friendly
* More likely to fight for LibreTaxi rights when it comes to regulations (Germany/EU jurisdiction)

## Technical roadmap (unordered)

* Make it safer for passengers and drivers
* Add Bitcoin integration
* Add drivers/passengers rating
* Add configuration based on zones and regions
* Add more vehicle types
* Make it easier to use and safer for moms/dads and children
* Make it easier to use for people with disabilities
* Add more translations
* Add integration (click) tests (and infrastructure) for Telegram platform
* Add delayed rides
* Refactoring, refactoring, refactoring

## Development guidelines

* [Installing Node.js](doc/NODEJS.md)
* [Getting started](doc/GETTING-STARTED.md)
* [Redis](doc/REDIS.md)
* [Esdoc](doc/ESDOC.md)
* [Contributing](doc/CONTRIBUTING.md)
* [Add translation](doc/TRANSLATE.md)

## Linux tweaks

This package is using unicode emojis. [Click here](https://github.com/eosrei/emojione-color-font#install-on-ubuntu-linux) to install them. Unfortunately, on Linux they are in one color in Terminal and in Atom editor. Update this doc if you were able to make them in color in Terminal and/or Atom editor.
