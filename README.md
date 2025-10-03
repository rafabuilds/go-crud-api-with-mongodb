# go-crud-api-with-mongodb

A robust CRUD RESTful API in **Go**, using **MongoDB** as the database. This project is a complete solution for building APIs, featuring containerization with **Docker**, authentication with **JWT**, and interactive documentation with **Swagger**.

---

## Technologies Used

* **Go (Golang):** The main programming language.
* **MongoDB:** A NoSQL database for data persistence.
* **Docker & Docker Compose:** For containerization and service orchestration.
* **JWT (JSON Web Tokens):** For user authentication and authorization.
* **Swagger:** For interactive documentation and visualization of API endpoints.

---

## Features

* **C**reate: Creation of new resources.
* **R**ead: Listing and searching for resources.
* **U**pdate: Updating existing resources.
* **D**elete: Deleting resources.
* **Authentication:** User login and JWT token validation.
* **Containerized Services:** The API and database run in separate containers, making the project portable.
* **API Documentation:** Accessible via the Swagger UI interface.

---

## How to Run the Project

### Prerequisites

Make sure you have **Docker** and **Docker Compose** installed on your machine.

### Steps

1.  Clone this repository:
    ```bash
    git clone [https://github.com/your-username/go-crud-api-with-mongodb.git](https://github.com/your-username/go-crud-api-with-mongodb.git)
    cd go-crud-api-with-mongodb
     ```

2.  Start the API and MongoDB containers:
    ```bash
    docker-compose up --build
    ```
    This will build your Go application image and start the services defined in `docker-compose.yml`.

3.  Access the API:
    * The API will be running at `http://localhost:8080`.
    * The interactive **Swagger** documentation can be accessed at `http://localhost:8080/swagger/index.html`.

---

## Project Structure


├── cmd/api/main.go          # Main entry point of the application

├── internal/

│   ├── handlers/            # Functions that handle HTTP requests


│   ├── models/              # Data structures (objects, schemas)


│   └── routes/              # Definition of API routes

├── pkg/

│   └── utils/               # Utility functions (DB connection, JWT)

├── Dockerfile               # Instructions to build the Go image

├── docker-compose.yml       # Container orchestration

├── go.mod                   # Go dependency manager

└── README.md                # This file



---

## API Endpoints

Access the **Swagger** documentation to see all available endpoints and test them directly.

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `POST` | `/api/v1/auth/login` | Authenticates a user and returns a JWT. |
| `GET` | `/api/v1/users` | Lists all users. |
| `POST` | `/api/v1/users` | Creates a new user. |
| `GET` | `/api/v1/users/{id}` | Finds a user by ID. |

---

## Contributions

Feel free to contribute to this project!

1.  Fork the repository.
2.  Create a new branch (`git checkout -b feature/new-feature`).
3.  Make your changes and commit (`git commit -am 'Adds new feature'`).
4.  Push to the branch (`git push origin feature/new-feature`).
5.  Open a Pull Request.

---

Made with 💙 by **Rafael Contreira, Backend Developer.*
