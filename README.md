# Starbase-Jukebox

Welcome to the wonderful world of programming-based music!  Find the initial setup chips and device images in the "Jukebox Setup" folder.  This entire system only uses basic chips so far.  I did not include a blueprint file since the entire parts list at the minimum is: 3x basic chips, 1x memory chip, chip storage, 2x Audio Signal Device MK1, 6 buttons, and power.  These can go anywhere in your ship's network, or slapped onto a battery for a grab-able setup.  You may add up to 4x more basic chips as song loaders.  If you want more song capacity, just add another memory module with more buttons and more tracks, you also have to add onto the SongSelector code.

When you want to play a song, copy the code from any of the Song loader scripts into a basic yolol chip.  If the Jukebox chips are in your yolol network then this should load the song into a track on the memory chip.  

If you are writing your own music I recommend using the transposer script.  It is a bit more complicated but makes things a lot easier if you read music.  Basically follow the format of some of the other transposed songs in that folder.  Spaces in those .txt files are the equivalent of rests, and it is written such that the smallest unit are eight notes.  If you see a "D " then that is a quarter note D as an example.  You do need to start a new line for every note change, but spaces can go on lines with notes.

If you are writing your own music and dont want to use the transposer, remember that you need to reverse the text of your song when putting it into a Song Loader yolol chip, because it reads it backwards.  A website like https://www.browserling.com/tools/text-reverse  will do that for you.  You can write it normally, just reverse it with this tool.  The chromatic octave is transcribed in the code such that A=a, A#=b, B=c, ... , C.=m (C. is the higher C).

The Double Track setup is in development, and the first song is being written for it.  This allows for parallel tracks to play and thus multiple notes at the same time.  Useful for more complicated songs.

The project's github: https://github.com/superwafflefry/Starbase-Jukebox

(Code that is not the same but a starting point in case you were curious about the history of this)
Github: https://github.com/Lumi-Virtual/YOLOL-Sketchbook/blob/main/SSP/SSP.yolol