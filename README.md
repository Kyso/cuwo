![cuwo](http://mp2.dk/cuwo/logo.png)
====

cuwo is an open server implementation for Cube World, written in Python.
It currently has the best protocol coverage among all the server projects out
there, and has features like

* Cross-platform support (Windows, Mac OS X, Linux, FreeBSD, what have you)
* File/console logging
* MOTD message
* Scripting (see the minimal welcome.py example)
* Advanced configuration
* Ban system
* Commands (/kick, /say, /whereis, /setclock, /kill, /stun. etc.)
* Rights management (/login password)
* IRC bot
* PvP script
* DDoS prevention
* Lower CPU requirements than normal server
* Master server on http://mp2.dk/cuwo
* Support for 40+ players
* ... and much more!

Running
=======

On Windows, see the 
[quick-start guide](https://github.com/matpow2/cuwo/wiki/Quickstart) for a 
quick way to get started.

On Linux/Mac OS X/FreeBSD/etc., make sure you have Python 2.7 and Twisted
installed on your machine, then run run_server.sh. 

Status
======

In terms of gameplay, the following has been implemented:
* Player join/leave
* Player movement and animations
* Magic/arrows/etc. relay
* Player hits on entities/other players
* Item pickup/drop
* Time management

A lot is still to be implemented gameplay-wise. Most importantly, NPCs and mobs
have not been implemented yet. We still need to rip out the terrain generator,
and once that's done, NPCs and mobs should be completely doable.

There is also a working MITM proxy that can inject packets. It's useful for
reverse-engineering the protocol and can be used as an alternative to a
standalone server.

There is also a working Cube World/Qubicle model converter. Find it in the 
'tools' folder.

FAQ
===

* **Q.** How do I pronounce 'cuwo'?

* **A.** 'coo-woo' (no, not 'kew-woh')

* **Q.** I am not a programmer, and I can't reverse-engineer anything. How do
         I help?

* **A.** We need people who can create end-user documentation as well! Have a
         look around, and see if anything is missing in the wiki.

* **Q.** What is a MITM proxy?

* **A.** A MITM proxy sits between your client and server, and can manipulate
         and inject packets. It's not really useful for the normal user, so
         use the regular cuwo server instead.

Special thanks
==============

Sarcen - help with protocol variables, scripting, anticheat

Perl - protocol RE

ZeZeene - web interface for master server

Kyle - master server JS

Kainzo - testing

uwee - protocol variables

Somer - help with some protocol variables

Favorlock - scripting and commands

SLoW - scripting

DRayX - encrypt.py and protocol RE

MAT4DOR - cub model details

Xaymar - RE and character details
