# SchedulAI: AI-Powered Task Scheduling App

## Project Overview

This project is an open-source, AI-powered task scheduling application with a web interface built using Vue.js, focusing on integration with Google Calendar and utilizing LLM-based scheduling algorithms.

## Tech Stack

- Frontend: Vue.js with TypeScript
- Backend: Node.js with Express
- Database: PostgreSQL
- AI/ML: TensorFlow.js for client-side ML, Python with Flask for server-side ML
- Containerization: Docker and Docker Compose

## Getting Started

### Prerequisites

- Docker and Docker Compose
- Git

### Installation and Setup with Docker

1. Clone the repository

   ```
   git clone https://github.com/your-username/ai-task-scheduler.git
   cd ai-task-scheduler
   ```

2. Build and start the Docker containers

   ```
   docker compose up --build -d
   ```

3. Access the application

   - Frontend: http://localhost:8080
   - Backend API: http://localhost:3000

4. To stop the containers
   ```
   docker compose down
   ```

### Development Workflow

- The source code for both frontend and backend is mounted as volumes in the Docker containers. This means you can make changes to the code on your host machine, and the changes will be reflected in the running containers.

- To view logs from the containers:

  ```
  docker compose logs
  ```

- To rebuild the containers after making changes to the Dockerfiles or docker-compose.yml:
  ```
  docker compose up --build -d
  ```

### Troubleshooting

If you encounter issues with the Docker setup:

1. Check the logs for each service:

   ```
   docker compose logs frontend
   docker compose logs backend
   docker compose logs db
   ```

2. Ensure all necessary ports are free on your host machine (8080 for frontend, 3000 for backend).

3. If changes aren't reflecting, try rebuilding the containers.

## Project Structure

```
ai-task-scheduler/
├── frontend/
│   ├── Dockerfile
│   └── ... (Vue.js app files)
├── backend/
│   ├── Dockerfile
│   └── ... (Node.js app files)
├── docker-compose.yml
└── README.md
```

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests.

## License

This project is licensed under the GNU GENERAL PUBLIC LICENSE - see the [LICENSE.md](LICENSE.md) file for details.
