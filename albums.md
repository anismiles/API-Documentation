# Albums

## Create an album
* `POST /albums`
* Arguments:
   * name
   * public `1 or 0`

*Note*: The Content-Type header must be defined: `Content-Type: application/x-www-form-urlencoded`.

Returns the following:
```json
{
   "id": "1794",
   "name": "hai",
   "hash": "h0du630Bta",
   "public": "1",
   "photos": "0"
}
```

## Get an album
* `GET /albums/30g7djMmSd`

Returns the following:
```json
{
   "id": "2",
   "name": "4St",
   "hash": "30g7djMmSd",
   "public": "1",
   "photos": "4"
}
```

## Update an album
* `PUT /albums/30g7djMmSd`
* Arguments:
   * name
   * public `1 or 0`

Returns the following:
```json
{
   "id": "1792",
   "name": "test",
   "hash": "39g7djMmSd",
   "public": "0",
   "photos": "4"
}
```

## Delete an album
* `DELETE /albums/30g7djMmSd`

Returns the following:
```json
{
   "message": "The album is succesfully deleted."
}
```

## Get all albums
* `GET /albums`

Returns the following:
```json
[
   {
      "id": "1",
      "name": "d",
      "hash": "r8RreQ9mLa",
      "public": "0",
      "photos": "3"
   },
   {
      "id": "5",
      "name": "hai",
      "hash": "h0du630Bta",
      "public": "1",
      "photos": "0"
   }
]
```

## Delete all albums
* `DELETE /albums`
* Argument (optional, only needed if you want to delete specific albums):
   * albums `album hashes separated with commas`

Returns the following:
```json
{
   "message": "The albums are succesfully deleted."
}
```