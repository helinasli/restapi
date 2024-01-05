# RESTful API using Golang

This repository contains a simple RESTful API written in Golang, utilizing a custom application framework, a MongoDB database connection, and basic routing.

## Setup PostgreSQL Docker Container

To set up a PostgreSQL Docker container, run the following commands:

```bash
docker run --name postapidb --env POSTGRES_PASSWORD=postgres -p 5432:5432 -d postgres
```

## Project Structure

- `main.go`: Entry point of the application, initializes the app, establishes a connection to MongoDB, and starts the HTTP server.

- `app/`: Package containing the application code and logic.
  - `app.go`: Defines the application structure and its components.
  - `router.go`: Implements the HTTP routing logic.

- `app/database/`: Package managing the database connection.
  - `db.go`: Defines the database structure and methods.

## Usage

1. Clone the repository.
2. Ensure that Golang and MongoDB are installed on your machine.
3. Run the application using `go run main.go`.
4. Access the API at `http://localhost:9000`.

## Dependencies

- MongoDB driver for Golang

## License

This project is licensed under the [MIT License](LICENSE).

