shpotify: A command-line interface to Spotify
=============================================

Copyright (c) 2012 Harish Narayanan

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
   * quit     = Quit Spotify.

