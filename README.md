# RPi-Jukebox-RFID
A jukebox for the Raspberry Pi, playing local audio files, playlists or even web streams triggered by RFID cards. All plug and play via USB, no soldering iron needed.

## Installation

Follow the instructions in the [`INSTALL.md`](docs/INSTALL.md) file in the `docs` folder.

## Acknoledgements

There are many, many, many inspiring suggestions and solutions on the web to bring together the idea of a jukebox with RFID cards. I want to mention a few of these that have inspired me.

* [Jeremy Lightsmith's rpi-jukebox](https://github.com/jeremylightsmith/rpi-jukebox) written in Python, using the mpg123 player
* [Marco Wiedemeyer's Raspberry Pi Jukebox für Kinder (German)](https://mwiedemeyer.de/blog/post/Raspberry-Pi-Jukebox-fur-Kinder) written in mono, using the MPD player
* [Marcus Nasarek's Kindgerechter Audioplayer mit dem Raspberry Pi (German)](http://www.raspberry-pi-geek.de/Magazin/2014/03/Kindgerechter-Audioplayer-mit-dem-Raspberry-Pi) triggered by QR codes via a camera instead of RFID cards, written in bash and using the xmms2 media player
* [Huy Do's jukebox4kids / Jukebox für Kinder](http://www.forum-raspberrypi.de/Thread-projekt-jukebox4kids-jukebox-fuer-kinder) written in Python, [the code is on github](https://github.com/hdo/jukebox4kids)
* [Francisco Sahli's Music Cards: RFID cards + Spotify + Raspberry Pi](https://fsahli.wordpress.com/2015/11/02/music-cards-rfid-cards-spotify-raspberry-pi/) written in python, playing songs from Spotify. The code [music-cards is on GitHub](https://github.com/fsahli/music-cards)
* [Willem van der Jagt's How I built an audio book reader for my nearly blind grandfather](http://willemvanderjagt.com/2014/08/16/audio-book-reader/) written in python and using the MDP player.

For my rendition of the RFID jukebox, I have used the python libraries from [Francisco Sahli](https://github.com/fsahli/music-cards) to register the RFID reader and read the ID from the cards with the python scripts `Reader.py` and `RegisterDevice.py`.

I also want to link to two proprietary and commercial projects, because they also inspired me. And they challenged me, because of their shortcomings in terms of openness and in the case of tonies, the lack of "ownership" of the audiobooks and plays you actually bought. However, both products are very well made.
* [tonies® - das neue Audiosystem für mehr Hör-Spiel-Spaß im Kinderzimmer. (German)](https://tonies.de/) You buy a plastic figure which then triggers the audiofile - which is served over the web.
* [Hörbert - a MP3 player controlled by buttons](https://hoerbert.com) In Germany this has already become a *classic*. They also started selling a DIY kit.

## Shopping list

Here is a list of equipment needed. Chances are that you will find most of it in the back of your drawers or at the bottom of some shoe box. Well, most of it, possibly not the RFID reader itself.

* [Raspberry Pi 3 Model B ](http://amzn.to/2ku0PU7) | You might be surprised how easy and affordable you can get an RPi second hand. Think about the planet before you buy a new one.
* [Contactless RFID IC Card Reader with USB Interface PLUS 5 Cards + 5 Key Fob](http://amzn.to/2kXkMjr) | This package is good value for money, because it gets you started, including everything plus 5 RFID cards and 5 key fobs. 
* [USB Stereo Speaker Set (6 Watt, 3,5mm jack, USB-powered) black](http://amzn.to/2kXrard) | This USB powered speaker set sounds good for its size, is good value for money and keeps this RPi project clean and without the need of a soldering iron :)
* [External USB Soundcard with Virtual Surround Sound, Plug & Play](http://amzn.to/2kXflBf) | The additional soundcard is optional. If you don't like the sound coming straight from the RPi jack, this is a good value for money USB soundcard.
* [USB A Male to Female Extenstion Cable with Switch On/Off](http://amzn.to/2kXflBf) | I placed this USB extension between the USB power adapter and the jukebox. This will allow you to switch the jukebox on and off easily.
* [USB 2.0 Hub 4-port bus powered USB Adapter](http://amzn.to/2kXeErv) | Depending on your setup, you will need none, one or two of these. If you are using the external USB powered speakers, you need one to make sure the speakers get enough power. If you want to use the additional USB soundcard and have an older RPi, you might need a second one to make sure you can connect enough devices with the RPi.
