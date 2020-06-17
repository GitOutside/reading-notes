# Web Storage
Cookies were designed to sotre small amounts of data for apps that reside on an individual's computer.
Cookies are slow, not secure, and limited to around 4KB of data.

## userData 
This allows webpages to store up to 64KB of data.
Then came LSO - Local Shared Objects, which store up to 100KB per domain.

## Google Gears
This can store unlimited amounts of data per domain in SQL database tables.

## HTML5 Storage
Allows storage of key/value pairs locally within web browser. Similar to cookies, but never transmitted to remote server
unless you purposefully send it. 

To check if a browser supports it, you can use [Moderizer](http://diveinto.html5doctor.com/detect.html#modernizr) to detect support for HTML% storage.

You store data on a named key, and you can retrieve the data with the same key.
 - Key is a string
 - Value can be strings, booleans, integers or floats. BUT it is stored as a string. Think parseInt and parseFloat.

 ## storage event
 You can trap the storage event, which is fired on the Window object when ```setItem()```, ```removeItem()```, or ```clear()``is called, but only if that invocation ***changes*** something. Storage event does not support addEventListener.