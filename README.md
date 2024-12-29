# Dicoding Node.js Web Server

![Node.js](https://img.shields.io/badge/Node.js-v14.17.0-green) ![License](https://img.shields.io/badge/license-MIT-brightgreen)

This project demonstrates how to build a simple web server using Node.js without any external frameworks. The project is part of the Dicoding "Belajar Membuat Aplikasi Back-End untuk Pemula" course and focuses on creating a web server that can handle HTTP requests, process data, and return appropriate responses.

---

## Features

- Create an HTTP server with Node.js
- Handle different HTTP methods (GET, POST, PUT, DELETE)
- Process incoming requests and send responses
- Serve static files
- Understand basic routing mechanisms

---

## Prerequisites

Ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v14.x or later)
- [npm](https://www.npmjs.com/) (v6.x or later)

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yorizpra/dicoding_nodejs-web-server.git
   ```

2. Navigate to the project directory:
   ```bash
   cd dicoding_nodejs-web-server
   ```

3. Install dependencies (if applicable):
   ```bash
   npm install
   ```

---

## Running the Application

1. Start the server:
   ```bash
   node server.js
   ```

2. The server will run at:
   ```
   http://localhost:5000
   ```

---

## API Endpoints

### 1. Home Route
- **URL**: `/`
- **Method**: `GET`
- **Response**:
  - `200 OK`: Welcome message.

### 2. About Route
- **URL**: `/about`
- **Method**: `GET`
- **Response**:
  - `200 OK`: About page message.

### 3. Add Data
- **URL**: `/data`
- **Method**: `POST`
- **Request Body**:
  ```json
  {
    "key": "value"
  }
  ```
- **Response**:
  - `201 Created`: Data successfully added.

### 4. Update Data
- **URL**: `/data/{id}`
- **Method**: `PUT`
- **Request Body**: Same as Add Data.
- **Response**:
  - `200 OK`: Data successfully updated.
  - `404 Not Found`: Data ID not found.

### 5. Delete Data
- **URL**: `/data/{id}`
- **Method**: `DELETE`
- **Response**:
  - `200 OK`: Data successfully deleted.
  - `404 Not Found`: Data ID not found.

---

## Project Structure

```
├── src
│   ├── handler.js          # Handles request processing
│   ├── routes.js           # Defines route configurations
│   ├── server.js           # Main server file
├── static                  # Static files (e.g., HTML, CSS)
├── package.json            # Project metadata and dependencies
└── README.md               # Project documentation
```

---

## Dependencies

No external dependencies are required for this project. It uses Node.js built-in modules such as `http` and `fs`.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- [Dicoding](https://www.dicoding.com/) for providing the learning platform.
- [Node.js](https://nodejs.org/) for its powerful runtime environment.

---

Feel free to contribute to this project by submitting issues or pull requests!
