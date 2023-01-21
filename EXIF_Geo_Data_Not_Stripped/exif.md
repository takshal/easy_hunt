# exif Geolocation data not stripped

<h4>Summary:</h4>
When a user uploads an image in abc.com, the uploaded image’s EXIF Geolocation Data does not gets stripped. As a result, anyone can get sensitive information of abc.com users like their Geolocation, their Device information like Device Name, Version, Software & Software version used etc.

<h5>where to test</h5>
1. you can test on profile image upload function
2. any other location where you can upload image

# steps to test

1. go to github and download image(https://github.com/ianare/exif-samples/blob/master/jpg/gps/DSCN0010.jpg)
2. upload image on website
3. find a uploaded image path 
4. open it (http://exif.regex.info/exif.cgi)
5. check still showing exif data or not


