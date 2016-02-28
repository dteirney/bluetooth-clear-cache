# Clear your Mac OS X Bluetooth Cache

The `bluetooth-clear-cache` script can be used to clear the Bluetooth cache on Mac OS X. It is based on instructions provided by the team that develop [Knock to Unlock](http://www.knocktounlock.com/).

**Note that you will need to pair existing Bluetooth devices with your Mac once the Bluetooth cache has been cleared.**

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

## Pair Existing Bluetooth Devices

When your Mac restarts, a new Bluetooth preference file will be created.

You will need to pair existing Bluetooth devices with your Mac again, e.g. your Bluetooth Keyboard, Trackpad, iPhone, etc. This should happen automatically when each Bluetooth device is discoverable and moves within range of the Mac because the ID for each device is still remembered by OS X even after clearing the Bluetooth cache.

Until each existing device is paired again it will appear with just the device ID in the Bluetooth panel of System Preferences, like below:

![Bluetooth System Preferences](/docs/bluetooth-system-preferences.png)

After pairing, the name of the device will be presented instead of the device ID.

## Done

Hopefully, whatever Bluetooth problems you had are gone!
