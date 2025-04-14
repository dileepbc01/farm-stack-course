# Farm-Tut Application

This project is a full-stack application consisting of a frontend (React), backend (FastAPI), and an Nginx reverse proxy. The application is containerized using Docker and orchestrated with Docker Compose.

## Requirements

Before running the application, ensure you have the following installed on your system:

1. **Docker**: [Install Docker](https://docs.docker.com/get-docker/)
2. **Docker Compose**: [Install Docker Compose](https://docs.docker.com/compose/install/)
3. **Node.js**: [Install Node.js](https://nodejs.org/) (for local frontend development)
4. **Python 3.10+**: [Install Python](https://www.python.org/downloads/) (for local backend development)
5. **Poetry**: [Install Poetry](https://python-poetry.org/docs/#installation) (for managing Python dependencies)

## How to Run

Follow these steps to run the application using Docker Compose:

1. Navigate to the project directory where the `compose.yaml` file is located.

2. Create a `.env` file in the root directory and add the MongoDB connection URI:
   ```env
   MONGO_URI=mongodb://<username>:<password>@<host>:<port>/<database>
   ```

3. Build and start the containers:
   ```bash
   docker-compose up --build
   ```