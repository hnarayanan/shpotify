shpotify: A command-line interface to Spotify
=============================================

Copyright (c) 2012--2014 Harish Narayanan

This is a simple Bash/Apple script to control Spotify from the
command line on a Mac. It can be used to remotely control Spotify
from other machines using SSH. In order to use it:

1. Make sure the 'spotify' file in this folder is executable::

     chmod +x spotify

2. Copy the file to a convenient location in your PATH
3. Run it by typing::

     spotify <option>

   where <option> is one of

   * status   = Shows Spotify's status, current track details.
   * play     = Start playing Spotify.
   * pause    = Pause Spotify.
   * toggle		= Toggle play/pause state of Spotify.
   * next     = Go to the next track.
   * prev     = Go to the previous track.
   * vol up   = Increase Spotify's volume by 10%
   * vol down = Increase Spotify's volume by 10%
   * vol #    = Set Spotify's volume to # [0-100]
   * share    = Copies the current track share URL to clipboard.
   * quit     = Quit Spotify.

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
