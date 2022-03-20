# Are you getting tired of the censorship?  

It is always interesting to gain insight into other cultures.  Russian’s invasion into Ukraine sparked a shift in the type of music that soldiers listen to.  

Essentially…

Regardless of what genre that you listen to, music pumps the brain with subliminal messages.  Guns, violence, war, all get tagged into playlists which influences people share.  Music conveys messages.  It’s called a mnemonic device.  

For this post, I need to take you back in time.  A few months ago, I was applying for a data science job and the interview challenge was to use the python library spotipy.  I was tasked to created a data pipeline to pull song details into a CSV file. This is faster than making an SQLite database.  

After creating a Spotify “app”, I set up a spotify account on their website.

![image](https://user-images.githubusercontent.com/23527755/159144161-02ddf865-6973-4dab-bbdc-4b690ea41b3f.png)

Then I set a key to open the door into spotify.  The CID is the app ID which tells my computer which computers to connect to.  The secret is the password.  Then we are in.

![image](https://user-images.githubusercontent.com/23527755/159144165-f8823b77-a6e8-4605-bdb9-9063e8dc4074.png)

There’s a balance between setting up code so that efficiency is high and using it.  Here, the songs are organized into albums but I need to get them by tracks.  I could run separate API calls to each song… ugh… who has time for that?  

I create an empty list that will hold the strings. Then populate it by indexing the JSON “track”.  I only care about the audio features and not the album art or year, for example.  I concatenated the list with all the tracks from the Russian War Songs playlist.
