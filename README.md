# shpotify

*shpotify* is a simple Bash/Apple script to control
 [Spotify](https://www.spotify.com) from the command line on a Mac.

## Installation and usage

You can quickly get started with shpotify by following a few simple
steps:

1. Fetch a copy of this repository, either with git or [download the
   zip archive](https://github.com/hnarayanan/shpotify/archive/master.zip).

2. Navigate to the folder where you fetched the repository (unzip if
   needed) and make sure the file called `spotify` is executable:
   ````
   cd shpotify
   chmod +x spotify
   ````

3. Copy the file `spotify` to a convenient location in your `PATH`, or
   set your `PATH` to include the folder where the file is located.

4. That's it! You can now use it to control Spotify with the following
   commands:
   ````
   spotify play                      Resumes playback where Spotify last left off
   spotify play [song name]          Finds a song by name and plays it
   spotify play album [album name]   Finds an album by name and plays it
   spotify play artist [artist name] Finds an artist by name and plays it
   spotify play list [playlist name] Finds a playlist by name and plays it

   spotify next                      Skips to the next song in a playlist
   spotify prev                      Returns to the previous song in a playlist
   spotify pos [time]                Jump to a specific time (in seconds) in the current song
   spotify pause                     Pauses/Resumes Spotify playback
   spotify quit                      Stops playback and quits Spotify

   spotify vol up                    Increases the volume by 10%
   spotify vol down                  Decreases the volume by 10%
   spotify vol [amount]              Sets the volume to an amount between 0 and 100

   spotify status                    Shows the play status, including the current song details
   spotify share                     Shows and copies the current song URL to the clipboard for sharing

   spotify toggle shuffle            Toggles shuffle playback mode
   spotify toggle repeat             Toggles repeat playback mode
   ````

## Authors and contributing

shpotify is primarily written and maintained by [Harish
Narayanan](https://harishnarayanan.org).

Since it's an open source project, it contains numerous contributions
from many helpful people, including:

* Jorge Colindres
* Thomas Pritchard
* iLan Epstein
* Gabriele Bonetti
* Sean Heller

If you're interested in contributing too, please consider addressing
some of the [issues people have previously
reported](https://github.com/hnarayanan/shpotify/issues) and
[submitting a pull
request](https://help.github.com/articles/using-pull-requests/). **Thank
you!**

## Copyright and license

Copyright (c) 2012–2015 [Harish Narayanan](https://harishnarayanan.org).

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
