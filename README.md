shpotify: A command-line interface to Spotify
=============================================

This is a simple Bash/Apple script to control Spotify from the command
line on a Mac. In order to use it:

1. Fetch a copy of this repository and make sure the `spotify` file in
   this folder is executable:

       chmod +x spotify

2. Copy the file to a convenient location in your `PATH`.

3. Run it by typing one of the following commands:

````
spotify play                    Resumes playback where Spotify last left off
spotify play [song name]        Searches for a song by name and plays it
spotify pause                   Pauses Spotify playback
spotify quit                    Stops playback and quits Spotify
spotify next                    Skips to the next track in the playlist
spotify prev                    Returns to the previous track in the playlist

spotify vol up                  Increase the volume by 10%
spotify vol down                Decrease the volume by 10%
spotify vol [value]             Set the volume to a value between 0 and 100

spotify status                  Shows the current play status including track details
spotify share                   Shows the current track URL and copies it to the clipboard for sharing

spotify toggle shuffle          Toggles shuffle playback mode
spotify toggle repeat           Toggles repeat playback mode

Need better interfaces:
Album and playlist playback etc.
spotify pos [value]             Needs better interface

````

Copyright (c) 2012–2015 Harish Narayanan <mail@harishnarayanan.org>

Contains helpful contributions from Jorge Colindres and Thomas Pritchard.

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
