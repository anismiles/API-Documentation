# Photo

## Create / upload a photo
* `POST /photo`
* Argument:
   * files `contents of the file`

*Note*: You might need to specify `Content-Type: multipart/form-data`.

Returns the following:
```json
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
```

## Get a photo
* `GET /photo/gV968r3bhk`

Returns the following:
```json
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
```

## Update a photo
* `PUT /photo/gV968r3bhk`
* Argument:
   * title

Returns the following:
```json
{
   "id": "163030",
   "title": "hello",
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
```

## Delete a photo
* `DELETE /photo/gV968r3bhk`

Returns the following:
```json
{
   "message": "The photo is succesfully deleted"
}
```