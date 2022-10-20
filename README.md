# sp

With this script you can easily use Spotify features via command line on Linux.

## Installation

All you need to do is save the sp file in any of the directories added to yout PATH, e.g. I put it in "/usr/bin".

## Features

You can easily see all the features with "sp help":
```
Usage: sp [command]
Control a running Spotify instance from the command line.

  sp play       - Play/pause Spotify
  sp pause      - Pause Spotify
  sp next       - Go to next track
  sp prev       - Go to previous track

  sp current    - Format the currently playing track
  sp metadata   - Dump the current track's metadata
  sp eval       - Return the metadata as a shell script

  sp art        - Print the URL to the current track's album artwork
  sp display    - Display the current album artwork with display
  
  sp feh        - Display the current album artwork with feh

  sp url        - Print the HTTP URL for the currently playing track
  sp clip       - Copy the HTTP URL to the X clipboard
  sp http       - Open the HTTP URL in a web browser

  sp open <uri> - Open a spotify: uri
  sp search <q> - Start playing the best search result for the given query
  sp pl <q>     - Search playlists, start playing the best search result for the given query, if there is a match

  sp version    - Show version information
  sp help       - Show this information

Any other argument will start a search (i.e. 'sp foo' will search for foo).
```

## Activate search feature

To activate the search feature you need to change the SP_ID and SP_SECRET variables. You can get these values by going to https://developer.spotify.com/dashboard, logging-in with your Spotify account and creating a new app; you can then copy your Client ID and Secret ID.

## Credits

I found this script online, first [here](https://gist.github.com/wandernauta/6800547) (by [wandernauta](https://github.com/wandernauta)) and then [here](https://gist.github.com/streetturtle/fa6258f3ff7b17747ee3) (by [streetturtle](https://github.com/streetturtle)), but the search feature was not working. I was able to fix it, so I decided to share it here. 
Big thanks to [olegrumiancev](https://github.com/olegrumiancev) for his contribution: he added the feature of searching on playlist with "sp pl <q>". 
