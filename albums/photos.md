# Photos

## Create / upload photos
* `POST /albums/88rh93489k/photos`
* Argument:
   * files `content of the files`

Returns the following:
```json
[
   {
      "id": "163030",
      "title": "Penguins",
      "file_name": "62de5288061eca6a9e296f1726810cca.jpg",
      "views": "1",
      "hash": "gV968r3bhk",
      "url": {
         "small": "http://static.dyp.im/gV968r3bhk/small/62de5288061eca6a9e296f1726810cca.jpg",
         "medium": "http://static.dyp.im/gV968r3bhk/medium/62de5288061eca6a9e296f1726810cca.jpg",
         "large": "http://static.dyp.im/gV968r3bhk/large/62de5288061eca6a9e296f1726810cca.jpg",
         "full": "http://static.dyp.im/gV968r3bhk/62de5288061eca6a9e296f1726810cca.jpg"
      }
   }
]
```

## Get all photos
* `GET /albums/88rh93489k/photos`

Returns the following:
```json
[
   {
      "photo_hash": "s6MmnvNc8U",
      "photo_file_name": "16e71df9978417eb10218b68d15308c7.jpg",
      "photo_id": "163027",
      "photo_title": "Tulips",
      "photo_views": "2",
      "url": {
         "small": "http://static.dyp.im/s6MmnvNc8U/small/16e71df9978417eb10218b68d15308c7.jpg",
         "medium": "http://static.dyp.im/s6MmnvNc8U/medium/16e71df9978417eb10218b68d15308c7.jpg",
         "large": "http://static.dyp.im/s6MmnvNc8U/large/16e71df9978417eb10218b68d15308c7.jpg",
         "full": "http://static.dyp.im/s6MmnvNc8U/16e71df9978417eb10218b68d15308c7.jpg"
      }
   }
]
```

## Delete all photos
* `DELETE /albums/88rh93489k/photos`
* Argument (optional, only needed if you want to delete specific photos):
   * photos `photo hashes separated with commas`

Returns the following:
```json
{
   "message": "The photos are succesfully deleted."
}
```

## Get a photo
* `GET /albums/88rh93489k/photos/s6MmnvNc8U`

Returns the following:
```json
{
   "id": "163027",
   "title": "Tulips",
   "file_name": "16e71df9978417eb10218b68d15308c7.jpg",
   "views": "2",
   "hash": "s6MmnvNc8U",
   "url": {
      "small": "http://static.dyp.im/s6MmnvNc8U/small/16e71df9978417eb10218b68d15308c7.jpg",
      "medium": "http://static.dyp.im/s6MmnvNc8U/medium/16e71df9978417eb10218b68d15308c7.jpg",
      "large": "http://static.dyp.im/s6MmnvNc8U/large/16e71df9978417eb10218b68d15308c7.jpg",
      "full": "http://static.dyp.im/s6MmnvNc8U/16e71df9978417eb10218b68d15308c7.jpg"
   }
}
```

## Update a photo
* `PUT /albums/88rh93489k/photos/s6MmnvNc8U`
* Argument:
   * title

Returns the following:
```json
{
   "id": "163027",
   "title": "A new name",
   "file_name": "16e71df9978417eb10218b68d15308c7.jpg",
   "views": "2",
   "hash": "s6MmnvNc8U",
   "url": {
      "small": "http://static.dyp.im/s6MmnvNc8U/small/16e71df9978417eb10218b68d15308c7.jpg",
      "medium": "http://static.dyp.im/s6MmnvNc8U/medium/16e71df9978417eb10218b68d15308c7.jpg",
      "large": "http://static.dyp.im/s6MmnvNc8U/large/16e71df9978417eb10218b68d15308c7.jpg",
      "full": "http://static.dyp.im/s6MmnvNc8U/16e71df9978417eb10218b68d15308c7.jpg"
   }
}
```

## Delete a photo
* `DELETE /albums/88rh93489k/photos/s6MmnvNc8U`

Returns the following:
```json
{
   "message": "The photo is succesfully deleted."
}
```