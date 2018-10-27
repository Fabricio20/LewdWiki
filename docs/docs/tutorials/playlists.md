Welcome to the playlist tutorial, here you will learn how to use LewdBot playlists.

### Listing your playlists

To list all your playlists, use `L!pl list`. This will list the name, along with the ID of all your playlists, plus the
default guild playlist.

### Modifying your playlist

To modify a playlist, it must be the active playlist of a guild. To do so, use

```javascript
L!pl use [id or name]
```

This will enable the selected playlist on the current guild. So to add a song, for example, simply use the `L!add` command.

**Note**: Once a playlist is active, all playing, adding, removing, clearing will take place on the active playlist.
Activating a playlist activates it for the whole server.

**Locking**: To prevent abuse, all user-playlists are locked by default. This means that users can _use_ your playlist but not _modify_ it.
To allow other users to modify your playlist you would run the share command:
```javascript
L!pl share [id or name] [true/false] 
``` 

### Deleting a playlist

To delete a playlist, simply use `L!pl delete [id or name]`.

**Note**: As the name implies, this command will _permanently_ delete the playlist, which means you _will_ lose all
songs in it.

### Creating a new playlist

To create a playlist, simply use `L!pl create [id or name]`.

**Note**: Non-premium users can only create one playlist. There is, however, no limit on the amount of songs
a playlist can have. (Don't abuse however - I'm watching...)

### Renaming a playlist

To rename your playlist, for the sake of organization, simply use `L!pl rename [name or id] [new name]`.