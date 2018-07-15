Installing json-server
json-server is a node module, and hence can be installed globally by typing the following at the command prompt:


   npm install json-server -g

If you are using OSX or Linux, use sudo at the front of the command. This will install json-server that can be started from the command line from any folder on your computer.

Configuring the Server
At any convenient location on your computer, create a new folder named json-server, and move to this folder.
Download the db.json file provided above to this folder.
Move to this folder in your terminal window, and type the following at the command prompt to start the server:


json-server --watch db.json -d 2000 -H 0.0.0.0

This should start up a server at port number 3000 on your machine. The data from this server can be accessed by typing the following addresses into your browser address bar:


http://localhost:3000/dishes
http://localhost:3000/promotions
http://localhost:3000/leaders
http://localhost:3000/feedback

Type these addresses into the browser address and see the JSON data being served up by the server. This data is obtained from the db.json file

Serving up the Images
The json-server also provides a static web server. Any resources that you put in a folder named public in the json-server folder above, will be served by the server at the following address:


  http://localhost:3000/

Shut down the server by typing ctrl-C in the terminal window.
Create a public folder in your json-server folder.
Download the images.zip file that we provide above, unzip it and move the images folder containing the images to the public folder.
Restart the json-server as we did before. Now your server will serve up the images for our NativeScript app. You can view these images by typing the following into your browser address bar:

http://localhost:3000/images/<image name>.png
