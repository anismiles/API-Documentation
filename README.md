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

## Methods
### /photo
<table>
	<tr>
		<th>HTTP Method</th>
		<th>Arguments</th>
		<th>Description</th>
	</tr>
	<tr>
		<td>POST</td>
		<td>
			<ul>
				<li>files</li>
			</ul>
		</td>
		<td>Upload a photo</td>
	</tr>
</table>

### /photo/[hash]
<table>
	<tr>
		<th>HTTP Method</th>
		<th>Arguments</th>
		<th>Description</th>
	</tr>
	<tr>
		<td>PUT</td>
		<td>
			<ul>
				<li>title</li>
			</ul>
		</td>
		<td>Update the photo</td>
	</tr>
	<tr>
		<td>GET</td>
		<td></td>
		<td>Get the photo data</td>
	</tr>
	<tr>
		<td>DELETE</td>
		<td></td>
		<td>Delete the photo</td>
	</tr>
</table>

### /albums
<table>
	<tr>
		<th>HTTP Method</th>
		<th>Arguments</th>
		<th>Description</th>
	</tr>
	<tr>
		<td>POST</td>
		<td>
			<ul>
				<li>name</li>
				<li>
					public
					<ul>
						<li>1 or 0</li>
					</ul>
				</li>
			</ul>
		</td>
		<td>Upload a photo</td>
	</tr>
	<tr>
		<td>GET</td>
		<td></td>
		<td>Get all the albums</td>
	</tr>
	<tr>
		<td>DELETE</td>
		<td>
			<ul>
				<li>
					albums
					<ul>
						<li>Optional</li>
						<li>Album hashes must be separated with commas</li>
					</ul>
				</li>
			</ul>
		</td>
		<td>Delete albums, all or specific ones</td>
	</tr>
</table>