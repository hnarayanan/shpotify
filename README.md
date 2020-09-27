# shpotify

*shpotify* is a simple Bash/Apple script to control
 [Spotify](https://www.spotify.com) from the command line on a Mac.

If you find this interesting, you should [follow me on
Twitter](https://twitter.com/copingbear) to learn about the other
things I do.

## Installation

[Download and install](http://www.spotify.com/download) the Spotify
desktop application if you haven’t already.

### With Homebrew

The easiest way to install shpotify is by using the [Homebrew package
manager](http://brew.sh):

````
brew install shpotify
````

### Manual installation

If you don’t use Homebrew, you can install the script manually by
following a few simple steps:

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

### Connecting to Spotify’s API

shpotify needs to connect to Spotify’s API in order to find music by
name. It is very likely you want this feature!

Spotify API has a 'public' part, for which developer/app are sufficient,
and it has a 'private' part, for which 'user authorization' is required.

To get this to work, you first need to sign up (or into) Spotify’s
developer site and [create an *Application*][spotify-dev]. Once you’ve
done so, you can find its `Client ID` and `Client Secret` values and
enter them into your shpotify config file at `${HOME}/.shpotify.cfg`.

Be sure to quote your values and don’t add any extra spaces. When
done, it should look like the following (but with your own values):

````
CLIENT_ID="abc01de2fghijk345lmnop"
CLIENT_SECRET="qr6stu789vwxyz"
````

If 'user authentication' is required, a spotify website will open in your
default browser asking for permission. After granting permission, a new
'localhost' site will be opened on port 8082 with a code in the URL. This code
is caught by Shpotify and is used to get the user-access code and user-refresh
token. From now it is possible to get information linked to your account, like
your playlists, history, devices, etc.

_note: thise page is supposed to automatically close, but that doesn't always
work properly._

## Usage

With shpotify you can control Spotify with the following commands:
````
spotify play                       Resumes playback where Spotify last left off.
spotify play <song name>           Finds a song by name and plays it.
spotify play album <album name>    Finds an album by name and plays it.
spotify play artist <artist name>  Finds an artist by name and plays it.
spotify play list <playlist name>  Finds a playlist by name and plays it.
spotify play uri <uri>             Play songs from specific uri.

spotify next                       Skips to the next song in a playlist.
spotify prev                       Returns to the previous song in a playlist.
spotify replay                     Replays the current track from the beginning.
spotify pos <time>                 Jump to a specific time (in seconds) in the current song.
spotify pause                      Pauses (or resumes) Spotify playback.
spotify stop                       Stops playback.
spotify quit                       Stops playback and quits Spotify.

spotify vol up                     Increases the volume by 10%.
spotify vol down                   Decreases the volume by 10%.
spotify vol <amount>               Sets the volume to an amount between 0 and 100.
spotify vol [show]                 Shows the current volume.

spotify status                     Shows the play status, including the current song details.
spotify status artist              Shows the currently playing artist.
spotify status album               Shows the currently playing album.
spotify status track               Shows the currently playing track.
spotify status liked <uri>*        Shows if a track or album is liked or not.

spotify share                      Displays the current song's Spotify URL and URI.
spotify share url                  Displays the current song's Spotify URL and copies it to the clipboard.
spotify share uri                  Displays the current song's Spotify URI and copies it to the clipboard.

spotify toggle shuffle             Toggles shuffle playback mode.
spotify toggle repeat              Toggles repeat playback mode.

spotify list uri <format> <uri>    List information about track, album or playlist by uri. Format in csv|tsv|text|html"
spotify list myalbums <format>*    List 50 of your last liked albums, format in csv|tsv|text|html";
spotify list mytracks <format>*    List 50 of your last liked songs, format in csv|tsv|text|html";
spotify list mine <format>*        List 'my' playlists (uri, title, public), format in csv|tsv|text|html";
spotify list history <format>*     List 30 last played tracks (uri, title, artist, album), format in csv|tsv|text|html

spotify like <uri>*                Like a song or album and add it to your library.";

spotify -v | --version             Shows the shpotify and spotify versions.";

* Please note that this requires authentication via a browser."
````

## Authors and contributing

shpotify is primarily written and maintained by [Harish
Narayanan](https://harishnarayanan.org).

Since it’s an open source project, it contains numerous contributions
from many helpful people, including:

* Jorge Colindres
* Thomas Pritchard
* iLan Epstein
* Gabriele Bonetti
* Sean Heller
* Eric Martin
* Peter Fonseca

If you’re interested in contributing too, please consider addressing
some of the [issues people have previously
reported](https://github.com/hnarayanan/shpotify/issues) and
[submitting a pull
request](https://help.github.com/articles/using-pull-requests/). **Thank
you!**

## Copyright and license

Copyright (c) 2012–2020 [Harish Narayanan](https://harishnarayanan.org).

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

[spotify-dev]: https://developer.spotify.com/my-applications/#!/applications/create
