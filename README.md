# SecureAPI

The project is a Node.js web server built using the Express.js framework. It includes middleware and routers for handling HTTP requests and responses, and implements CORS for securing the site from unauthorized access. The server also generates API endpoints to check the authorization of users, using JSON Web Tokens (JWTs) and Thunderclient for testing.

## Getting Started

To get started with this project, follow the instructions below.

### Prerequisites

Before running the server, you will need to have the following software installed on your machine:

- Node.js
- NPM

### Installation

To install the project, follow these steps:

1. Clone the repository to your local machine using the command `git clone <repository-url>`.
2. Navigate to the project directory using the command `cd <project-directory>`.
3. Install the project dependencies using the command `npm install`.

### Usage

To start the server, use the command `npm run start`. This will start the server and listen for incoming requests on port 3500. If you want to run the server in development mode and automatically restart the server when changes are made to the code, use the command `npm run dev`.

### Testing

To test the API endpoints, we use Thunderclient. First, start the server by running `npm run start`, then open Thunderclient and import the API requests from the `requests` directory. You can then use these requests to test the API endpoints.

### Authorization

To protect the server from unauthorized access, we use JSON Web Tokens (JWTs) to generate access and refresh tokens. The server sets the access token as an HttpOnly cookie, which can only be accessed by the server and not by client-side JavaScript. The refresh token is sent as a JSON object in the response body, and can be used to generate a new access token when the current one expires.

### CORS

Cross-Origin Resource Sharing (CORS) is implemented to secure the site from unauthorized access. The server sets the `Access-Control-Allow-Origin` header to allow requests from specified origins, and also sets the `Access-Control-Allow-Methods` header to specify which HTTP methods are allowed.

## Contributing

Contributions to this project are welcome! If you find a bug or would like to suggest a new feature, please open an issue in the repository. If you would like to contribute code, please open a pull request and we will review it as soon as possible.
