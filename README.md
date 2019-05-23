# OMG Sounds

A cross origin accessible library of sounds for Web Audio API.

## Background

OpenMusic.Gallery (OMG) is a web platform for music. Rather than storing audio files like MP3 or WAV, a song in OMG is stored as JSON and contains links to smaller audio files, such as a snare drum, or a bass note. 

There are hundreds of websites that offer free audio files. That means the sound files OMG can use has to be in the millions, right? Just plug in a URL to any audio file on the internet, and the user doesn't have download or host the file, yet it's immediately available to the user and whoever they share it with. Right?

## The Problem

Wrong. None of the dozens of websites that I've tried allow:

1. access to the raw file
2. without a login
3. without a developer key
4. with HTTPS
5. with CORS allowed

In order to sequence a sound, the browser has to be able to get the raw file from a remote server, which is usually blocked by CORS. 

I have setup my own servers to allow this, but the sounds on my server don't number in the millions like the internet at large. So close. So far away.

## SoundFonts

I found this repo: https://github.com/gleitz/midi-js-soundfonts

Which has a few hundred sounds, which is cool, and in the notes I found this:

* You can fetch Soundfont files directly from this repository, so you can access them directly from a browser. Use the prefix URL following by the instrument name. For example: http://gleitz.github.io/midi-js-soundfonts/FluidR3_GM/marimba-mp3.js

Woohoo! GitHub Pages allows cross origin requests!

I had tried DropBox in the past, and they had a "Public" folder at one point that worked for me. But GitHub is even better. 

## OMG Sounds

So here is a repo for storing the small building blocks of audio that OMG can use to make music.

And below is a list of sites that have been tested.

Feel free to contribute!

----

## Websites that work

GitHub Pages

## Websites that don't work

### login to download

https://freesound.org/
https://www.zapsplat.com/
https://www.soundeffectsplus.com
https://www.audioblocks.com
https://www.soundsnap.com
https://www.audiomicro.com
https://www.freesfx.co.uk
http://www.soundgator.com
https://www.soundeffectsforfree.com


### links, but no cors or https

http://soundbible.com
https://www.pacdv.com/
https://www.soundjay.com
http://www.moviewavs.com
http://wav-sounds.com/
http://www.wavsource.com
http://www.talkingwav.com
http://www.dailywav.com
https://www.noiseforfun.com
http://bbcsfx.acropolis.org.uk
http://www.grsites.com/archive/sounds/
https://www.partnersinrhyme.com/pir/PIRsfx.shtml
http://www.findsounds.com

### zip files

http://www.orangefreesounds.com
https://www.sounds4email.com/

### URLs misdirected?

https://www.freesoundeffects.com





