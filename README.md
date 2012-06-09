# CloudBot/DEV

## About

CloudBot is a Python IRC bot very heavily based on [Skybot](http://git.io/skybot) by [rmmh](http://git.io/rmmh).  

### Goals

* Easy to use wrapper
* Intuitive configuration
* Fully controlled from IRC
* Fully compatable with existing skybot plugins
* Easily extendable
  * Thorough documentation
  * Cross-platform
* Muti-threaded, efficient
  * Automatic reloading
  * Little boilerplate

## Download

Get CloudBot at [git.io/getcloudbotirc](http://git.io/getcloudbotirc "Get CloudBot from Github!").

Unzip the resulting file, and continue to read this document.

## Install

Before you can run the bot, you need to install a few Python modules. These are `lXML`, `Enchant`, `urllib3`, and `BeautifulSoup`.  These can be installed with `pip` (The Python package manager), or `easy_install` (A more basic version of `pip`):

`[sudo] pip install lxml pyenchant urllib3 beautifulsoup`

or

`[sudo] easy_install lxml pyenchant urllib3 beautifulsoup`

### Installing `pip`

```shell
curl -O http://python-distribute.org/distribute_setup.py
python distribute_setup.py
easy_install pip
```

(If you use Windows and don't want to set up pip, you can also find `exe` installers on the internet.)

## Running

Once you have installed the required dependencies, there are two ways you can run the bot:
### Launcher

The launcher will start the bot as a background process, and allow the bot to close and restart itself. This is only supported on unix-like machines (not Windows).

For the launcher to work properly, install `screen`, or `daemon` (daemon is recommended) :

`apt-get install screen`

`apt-get install daemon`

Once you have installed either `screen` or `daemon`, run the start command:

`./cloudbot start`

It will generate a default config for you.  Once you have edited the config, run it again with the same command:

`./cloudbot start`

This will start up your bot as a background process. To stop it, use `./cloudbot stop`. (Config docs at the [wiki](http://git.io/cloudbotircconfig))

### Manually

To manually run the bot and get debug output, run it with:

`python bot.py`

On Windows you can usually just double-click the `bot.py` file to start the bot, as long as you have Python installed correctly.

(note that running it without the launcher will break the restart and stop commands)

## Documentation

To configure your CloudBot, visit the [Config Wiki Page](http://git.io/cloudbotircconfig).

To write your own plugins, visit the [Plugin Wiki Page](http://git.io/cloudbotircplugins).

More at the [Wiki Main Page](http://git.io/cloudbotircwiki).

## Support

The developers reside in [#CloudBot](irc://irc.esper.net/cloudbot) on [EsperNet](http://esper.net) and would be glad to help you.

If you think you have found a bug/have a idea/suggestion, please **open a issue** here on Github.

## Example CloudBots

The developers of CloudBot run two CloudBots on [Espernet](http://esper.net).

They can both be found in [#CloudBot](irc://irc.esper.net/cloudbot "Connect via IRC to #CloudBot on irc.esper.net).

**mau5bot** is the semi-stable bot, and runs on the latest stable development version of CloudBot. (mau5bot is running on **Ubuntu Server** *Oneric Ocelot/11.10* with **Python** *2.7.2*)

**neerbot** is the unstable bot, and runs on the latest(ish) development version of CloudBot. (neerbot is running on **Debian** *Wheezy/Testing* with **Python** *2.7.2*)

## Requirements

CloudBot runs on **Python** *2.7.x*. It is developed on **Debian** *Wheezy/Testing* and **Ubuntu** *11.10* with **Python** *2.7.2*.

It **requires Python modules** `lXML`, `BeautifulSoup` and `Enchant`, `psutil`, and `HTTPlib2`.

The programs `daemon` or `screen` are recomended for the wrapper to run optimaly.

**Windows** users: Windows compatibility with the wrapper and some plugins is **broken** (such as ping), but we do intend to add it.³

## License
CloudBot is **licensed** under the **GPL v3** license. The terms are as follows.
    
    CloudBot/DEV

    Copyright © 2011-2012 Luke Rogers / ClouDev - <[cloudev.github.com](http://cloudev.github.com)>

    CloudBot is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    CloudBot is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with CloudBot.  If not, see <http://www.gnu.org/licenses/>.

## Notes

³ eventually
