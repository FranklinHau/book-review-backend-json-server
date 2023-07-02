# Book Review App Backend

This is the backend for the Book Review App. It uses a simple JSON file as a database to store information about books and their reviews.

## Database Structure

The database is a JSON file named db.json that contains an array of books. Each book is an object with the following properties:

- title: The title of the book.
- author: The author of the book.
- year: The year the book was published (as a number).
- description: A description of the book.
- reviews: An array of reviews for the book. Each review is an object with a text property for the review text and a rating property for the review rating (as a number between 1 and 5).
- id: A unique identifier for the book.

Here is an example of what the db.json file might look like:

```
{
  "books": [
    {
      "title": "The Teachings of Don Juan",
      "author": "Carlos Castaneda",
      "year": "1985",
      "description": "A story of a remarkable journey: the first awesome steps on the road to becoming a 'man of knowledge'",
      "reviews": [
        {
          "text": "\"Extraordinary in every sense of the word.\" ― The New York Times",
          "rating": 5
        },
        {
          "text": "Must read to understand the path of a warrior -Franklin",
          "rating": 4
        },
        {
          "text": "It sucks!! --theNegativeFamily",
          "rating": 4
        }
      ],
      "id": 1
    },
    ...
  ]
}

```
## Usage

To use the backend, you can make HTTP requests to the server. The server uses the following routes:

- GET /books: Returns an array of all books.
- GET /books/:id: Returns the book with the specified ID.
- POST /books: Adds a new book. The body of the request should be a JSON object representing the book.
- PUT /books/:id: Updates the book with the specified ID. The body of the request should be a JSON object representing the updated book.
- DELETE /books/:id: Deletes the book with the specified ID.

Each book object should have a title, author, year, description, and reviews property. The reviews property should be an array of review objects, and each review object should have a text and rating property.

## Installation


Before you can install the backend, you need to have Node.js and npm installed on your machine. Once you have those installed, you can clone the repository and install the dependencies with npm:

To install the backend, you can clone the repository and install the dependencies with npm:

git clone https://github.com/your-username/book-review-app-backend.git
cd book-review-app-backend
npm install

Then, you can start the server with npm start. The server will run on http://localhost:3001.

## Contributing

Pull requests are welcome. To make a pull request, fork the repository, create a new branch, make your changes, and then submit a pull request. For major changes, please open an issue first to discuss what you would like to change.

## Acknowledgment

Amazon Books: https://www.amazon.com/

## License
MIT