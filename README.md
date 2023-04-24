# GO-Movies-APP
This is a simple REST API for managing a collection of movies, implemented in Go using the net/http and github.com/gorilla/mux packages. It includes five routes:

GET /movies: retrieves all movies in the collection and returns them as a JSON array.
GET /movies/{id}: retrieves a single movie by ID and returns it as a JSON object.
POST /movies: creates a new movie in the collection based on the JSON object provided in the request body, and returns the newly created movie as a JSON object.
PUT /movies/{id}: updates an existing movie in the collection with the JSON object provided in the request body, and returns the updated movie as a JSON object.
DELETE /movies/{id}: deletes an existing movie from the collection by ID, and returns the remaining movies in the collection as a JSON array.
Each movie in the collection is represented as a JSON object with the following fields: id (string), isbn (string), title (string), and director (an embedded JSON object with firstname and lastname fields).

The rand package is used to generate unique IDs for new movies, and the log package is used for logging errors.

Feel free to use this code as a starting point for your own Go REST APIs!
