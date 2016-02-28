# Clear your Mac OS X Bluetooth Cache

Use the `bluetooth-clear-cache` script to clear the Bluetooth cache on Mac OS X. Based on instructions provided by the team that develop [Knock to Unlock](http://www.knocktounlock.com/).

**Note: you will need to rediscover existing Bluetooth devices paired with your Mac after clearing the Bluetooth cache.**

# Pre-Requisites

## blueutil

[blueutil](https://github.com/toy/blueutil), which is very easy to install using [Homebrew](http://brew.sh/).

    $ brew install blueutil

# Instructions

## Execute Script

The script requires admin privileges.

    $ sudo ./bluetooth-clear-cache

## Restart Mac

    $ shutdown -r now

## Rediscover Existing Bluetooth Devices

When your Mac restarts, a new Bluetooth preference file will be created.

Until each existing device, e.g. your Bluetooth Keyboard, Trackpad, iPhone, etc. is rediscovered it will appear with its device ID in the Bluetooth panel of System Preferences:

![Bluetooth System Preferences](/docs/bluetooth-system-preferences.png)

Rediscovery should happen automatically when each Bluetooth device is discoverable and moves within range of your Mac. After rediscovery, the device name will be presented instead of its ID.

## Done

Hopefully, whatever Bluetooth problems you had are gone!
