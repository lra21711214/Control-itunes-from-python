# What is Control-itunes-from-python?
Control-itunes-from-python is a program that allows you to control itunes(Music) from python.
# Install
1. download file<br>
```(Your project)$ curl -OL https://raw.githubusercontent.com/lra21711214/Control-itunes-from-python/master/control.py```

2. import
```from control import Control,Get_data```

# use
|Function|document|
|:---:|:---:|
|Control.play()|Play music|
|Control.pause()|Pause music|
|Control.playpause()|If the music is playing, stop the music and if the music is stopped play the music.|
|Control.stop()|Stop music|
|Control.next_track()|Play next track|
|Control.back_track()|Play from beginning of track.|
|Control.previous_track()|Play previous track|
|Control.play_list(play list name)|Plays the specified playlist|
|Get_data.current_track()|Get current track name|
|Get_data.current_track_artist()|Get current track artist name|
|Get_data.current_track_album()|Get current track album name|
|Get_data.current_all()|Get current track data(track name, artist name, album name) and return json|

# examples
```
from control import Control,Get_data

Control.play() ///play music

playlist_name = 'New Music Mix'
Control.play_list(playlist_name) ///play 'New Music Mix'

current_track = Get_data.current_track()
print(current_track) /// print current track
```
# Warning
This program only works on Mac(macOS 10.15 Catalina or later)
