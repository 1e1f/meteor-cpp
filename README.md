# meteor-cpp

A C++ [DDP](https://github.com/meteor/meteor/blob/master/packages/livedata/DDP.md) interface

Connect small or embedded devices to your Meteor Galaxy

## Status
* Connecting to both ws + wss endpoints using SSL
* only tested on OSX, ubuntu droplet next, windows not on roadmap yet.

## Dependencies
* Biicode dependency manager provides
* [boost](http://www.boost.org/) (`system` and `random` libs)
* [websocketcpp](https://github.com/zaphoyd/websocketpp)

## Install

Install BiiCode for OSX etc.
```
https://www.biicode.com/downloads
```

Install BiiCode on your droplet
```
nano /etc/apt/sources.list.d/biicode.list
deb http://apt.biicode.com trusty main
sudo wget -O /etc/apt/trusted.gpg.d/biicode.gpg http://apt.biicode.com/keyring.gpg
sudo apt-get update
sudo apt-get -y install biicode
bii setup:cpp
```

## Build

Now you've got biicode and this repo, so just
```
bii configure
bii build
```

## Run
```
bin/exceutable
```
