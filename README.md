# Request Header Parser Microservice

This project is the [exam](https://www.freecodecamp.org/learn/apis-and-microservices/apis-and-microservices-projects/request-header-parser-microservice
) part of the freeCodeCamp Back End Development and APIs curriculum. It is a Request Header Parser Microservice built using Node.js and Express. The application provides an API endpoint that returns the IP address, preferred languages, and system information of the user making the request.The structure of the project including the index.HTML was cloned from freeCodeCamp, I completed the index.js code.

You can view the live demo of the project [here](https://headparser-513880413aff.herokuapp.com/).

## Table of Contents

- Introduction
- Features
- [Technologies Used](#technologies-used)
- [Setup and Installation](#setup-and-installation)
- Usage
- [Project Structure](#project-structure)
- [API Endpoints](#api-endpoints)
- Troubleshooting
- Contributing
- License

## Introduction

The Request Header Parser Microservice is a web application that provides a simple API for returning user information based on request headers. It is built using Node.js and Express. This project is part of the freeCodeCamp Back End Development and APIs curriculum.

## Features

- **IP Address**: Retrieve the IP address of the user making the request.
- **Language**: Retrieve the preferred languages of the user.
- **System Information**: Retrieve the system information (user-agent) of the user.
- **CORS Enabled**: Allows cross-origin requests for remote testing.

## Technologies Used

- **Node.js**: JavaScript runtime environment.
- **Express**: Web framework for Node.js.
- **CORS**: Middleware for enabling CORS.
- **Dotenv**: Module for loading environment variables.

## Setup and Installation

To set up and run this project locally, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/request-header-parser-microservice.git
    cd request-header-parser-microservice
    ```

2. **Install dependencies**:
    ```bash
    npm install
    ```

3. **Create a `.env` file**:
    Create a `.env` file in the root directory and add the following:
    ```env
    PORT=3000
    ```

4. **Start the server**:
    ```bash
    npm start
    ```

5. **Open the application**:
    Open your web browser and go to [`http://localhost:3000`](http://localhost:3000).

## Usage

- **Get User Information**: Access the endpoint `/api/whoami` to get the IP address, preferred languages, and system information of the user making the request.

## Project Structure

```
request-header-parser-microservice/
│
├── public/                 # Public assets
│   ├── index.html          # Main HTML file
│   └── ...
│
├── views/                  # View templates
│   ├── index.html          # Main HTML file
│   └── ...
│
├── index.js                # Main server file
├── package.json            # Project dependencies and scripts
└── README.md               # Project documentation
```

## API Endpoints

- **GET `/api/hello`**: Returns a greeting message.
  - Response: `{ "greeting": "hello API" }`

- **GET `/api/whoami`**: Returns the IP address, preferred languages, and system information of the user making the request.
  - Response: `{ "ipaddress": "<IP address>", "language": "<preferred languages>", "software": "<system information>" }`

## Troubleshooting

If port 3000 is already in use, you can find the process ID (PID) and kill it using the following steps:

1. **Find the PID**:
    ```bash
    lsof -i :3000
    ```

    This command will list the processes using port 3000. Look for the PID in the output.

2. **Kill the process**:
    ```bash
    kill -9 <PID>
    ```

    Replace `<PID>` with the actual process ID you found in the previous step.

3. **Restart the server**:
    ```bash
    npm start
    ```

## Contributing

Contributions are welcome! If you have any suggestions or improvements, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

Thank you for checking out my Request Header Parser Microservice project! If you have any questions or feedback, feel free to reach out.
