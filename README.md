# Airship
Airship is a Python-based program to synchronize game saves between clouds, such as iCloud (for iOS) and Steam Cloud (for Steam).

## Downloading and installing

Before installing and running Airship, you must install these dependencies.

- All functionality depends on having Python version 2.6 or above installed (3.4 or above works too). Your operating system may have Python installed already; to check, type `python -V` into your terminal or command line. Otherwise, [download Python](https://www.python.org/downloads).
- It is *required* to install Airship through `pip`. [Download `pip`](https://pip.pypa.io/en/stable/installing.html#install-pip).
- Steam Cloud functionality depends on having Steam installed, logged in, and running while Airship is running. [Download Steam](https://store.steampowered.com/about).
- iCloud functionality depends on running Airship on OS X 10.10 Yosemite or above, being logged into iCloud, and having iCloud Drive synchronization enabled in System Preferences.

Download the latest release by running `pip install airship` and adding appropriate modules (like `pip install airship airship-steamcloud airship-icloud`).

## Using
To use, simply run `airship`.

For instructions on how to run Airship on a schedule, see the wiki page [Automatically running Airship](https://github.com/aarzee/airship/wiki/Automatically-running-Airship).

Airship will not synchronize a game if a cloud service is functioning, but has no files for the game. (This does not include clouds which are not active, or do not support the game). This is to prevent data loss in the event that a cloud service is somehow unavailable or otherwise does not have a local copy of the files. Before using Airship, please create a save file on all clouds you intend to use, and make sure the one that you want synchronized is the one last opened.

## Supported games
+ The Banner Saga ([Steam Cloud](http://store.steampowered.com/app/237990/), [iCloud](https://itunes.apple.com/us/app/banner-saga/id911006986))
