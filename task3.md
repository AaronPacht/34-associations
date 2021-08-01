Fork and clone this [repo](https://github.com/webdev-june-2021/34-associations). It is using the same db as chinook. If you get an error when connecting to db. Make sure to start the psql db by running
``` sudo -u postgres psql ```

## Questions

 

Make use of the methods added to your models by the associations in order to answer the following questions.
The Rails guide on associations can remind you what those methods are.

1. Find the album titled "Vinicius De Moraes", and then use an association-provided method to find all its
tracks.

Album.where(title:"Vinicius De Moraes")[0].tracks

2. Find the artist called "Philip Glass Ensemble", and then use an association-provided method to find all
their albums.

Artist.where(name:"Philip Glass Ensemble")[0].albums

3. Find the "Brazilian Music" playlist and then use an association-provided method to find all its tracks.

Playlist.where(name:"Brazilian Music")[0].tracks

4. Find the "Jazz" genre and then use an association-provided method to find all its tracks.

Genre.where(name:"Jazz")[0].tracks

5. Find the track "My Time After Awhile” and then use an association-provided method to find its genre.

Track.where(name:"My Time After Awhile")[0].genre

6. Use an association-provided method to find the media type of that same track.

Track.where(name:"My Time After Awhile")[0].media_type

7. Use an association-provided method to find the album that track appears on.


Track.where(name:"My Time After Awhile")[0].album