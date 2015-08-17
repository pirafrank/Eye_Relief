# Eye Relief

A very nimble utility to remember you to give your eyes a break.

## Why

I spend a lot of time programming and it's hard to track time to apply the [20-20-20 rule](http://lifehacker.com/5591835/reduce-computer-caused-eye-strain-with-the-20-20-20-rule).

## How it works

A short bash script is copied in ```/usr/local/bin``` and it is executed every 8 minutes by the built-in OS X utility *Launchd* (an Apple equivalent of Linux crontab).

Every 20 minutes it sends a notification as a reminder for you. 

That's why it's very nimble: it uses what's OS X already has!

## Warranty

Although the 20-20-20 rule is widely known, this utility is given WITHOUT ANY KIND OF WARRANTY on your health.

## Requirements

OS X 10.8 or above (due the need of notification center!). 

Tested on Mavericks and Yosemite.

## Installation

Step 0: download the repo as zip file, then unzip it. Open terminal in newly unzipped folder.

Step 1: `sudo cp eyerelief /usr/local/bin/eyerelief`

Step 2: `sudo chmod +x /usr/local/bin/eyerelief`

Step 3: `cp com.fpira.eyerelief.plist ~/Library/LaunchAgents/`

Step 4: `launchctl load ~/Library/LaunchAgents/com.fpira.eyerelief.plist `

## What's next

- Installer (.pkg)
- ON/OFF toggle option
- User's customization: Battery ranges ?
- Linux support ?

## License
The software in this repository are released under the GNU GPLv3 License by Francesco Pira (dev[at]fpira[dot]com, fpira.com). You can read the terms of the license [here](http://www.gnu.org/licenses/gpl-3.0.html).
