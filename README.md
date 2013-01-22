# DRAFT: DumpYourPhoto API Documentation

## Making a request
The API can be found at `https://api.dumpyourphoto.com/v1`. 
An API key must be specified on every API call, e.g.: `https://api.dumpyourphoto.com/v1/photo?api_key=yourkeyhere`. 
The standard response format is JSON, you can specify the format by adding `.xml`, `.json` or `.csv` at the end of the url, 
e.g.: `https://api.dumpyourphoto.com/v1/photo/somerandomhash.json?api_key=yourkeyhere`.

## Table of Contents
* [Photo](photo.md)
* [Albums](albums.md)
* [Photos](album/photos.php)