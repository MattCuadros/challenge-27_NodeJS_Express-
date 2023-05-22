> # Challenge #27 - **NodeJS - Express - My Repertoire**

---

In this Challenge, i used NodeJs and Express.js Server that handles CRUD operations (Create, Read, Update, Delete) for a collection of songs stored in a JSON file called "repertoire.json".

Here's a breakdown of the code:

Importing Dependencies:

express: Imports the Express.js framework for building web applications.
nanoid: Imports the nanoid function, which generates unique IDs for the songs.
readFile, writeFile: Imports functions from the Node.js fs/promises module for reading and writing files asynchronously.
Creating the Express App:

The express function is called to create an instance of the Express application.
The app uses express.json() middleware to parse incoming JSON data.
Setting up the Server:

The server is set to listen on the specified port (either the environment variable PORT or port 3000).
A console log message is printed when the server starts.
Handling Routes:

The root route ("/") responds with the content of the "index.html" file.
The "/canciones" route responds with the content of the "repertoire.json" file.
The "/canciones/:id" route handles a GET request for a specific song ID. It reads the "repertoire.json" file, finds the song with the matching ID, and responds with the song if found or a 404 error message if not found.
The "/canciones" route handles a POST request for adding a new song. It extracts the song data from the request body, generates a new ID using nanoid, reads the "repertoire.json" file, adds the new song object to the data array, and writes the updated data back to the file. It then responds with a success message and the new song object.
The "/canciones/:id" route handles a DELETE request for deleting a song. It reads the "repertoire.json" file, filters out the song with the matching ID, writes the updated data back to the file, and responds with a success message and the deleted song object.
The "/canciones/:id" route handles a PUT request for updating a song. It extracts the updated song data from the request body, checks if all the required fields are present, reads the "repertoire.json" file, updates the song object with the matching ID, writes the updated data back to the file, and responds with a success message and the updated song object.


---

###### Contact me in:

> - :bust_in_silhouette: Matias Cuadros
>   -:telephone_receiver: +569 4154 9653
>   -:email: <a href="mailto:mcuadrose@gmail.com" target="_blank">mcuadrose@gmail.com</a>

---

> ###### :warning: _All Rights Reserved - Visit my :briefcase: Briefcase in_ <a href="https://mattcuadros.github.io/" target="_blank">https://mattcuadros.github.io/</a> :copyright:
