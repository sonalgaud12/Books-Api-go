
# Book Management API

## Overview
This project is a simple Book Management API built using the Go programming language and the Gin web framework. It provides endpoints to perform basic CRUD operations on a collection of books, such as retrieving book details, adding new books, and updating book quantities for checkout and return operations.

## Features
- Retrieve a list of all books.
- Retrieve a book by its ID.
- Add a new book to the collection.
- Checkout a book (reduce quantity).
- Return a book (increase quantity).

## Endpoints

| Method | Endpoint       | Description                         |
|--------|---------------|-------------------------------------|
| GET    | `/books`       | Get a list of all books.            |
| GET    | `/books/:id`   | Get details of a specific book.     |
| POST   | `/books`       | Add a new book to the collection.   |
| PATCH  | `/checkout`    | Checkout a book by ID (decrease quantity). |
| PATCH  | `/return`      | Return a book by ID (increase quantity). |

## Technologies Used
- **Programming Language:** Go
- **Web Framework:** Gin

## Prerequisites
- Install [Go](https://go.dev/dl/)
- Install dependencies:
  ```sh
  go mod init books-api
  go get -u github.com/gin-gonic/gin
  ```

## Running the Application
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/book-management-api.git
   ```
2. Navigate to the project directory:
   ```sh
   cd book-management-api
   ```
3. Run the application:
   ```sh
   go run main.go
   ```
4. The API will be available at `http://localhost:8080`

## Example JSON Request for Adding a Book
```json
{
    "id": "4",
    "title": "Hamlet",
    "author": "William Shakespeare",
    "quantity": 2
}
```

## Operating System Used
This project has been tested and developed on:
- Windows
- Linux
- macOS

## Contribution
Feel free to fork the repository, make improvements, and submit pull requests.

## License
This project is licensed under the MIT License.

