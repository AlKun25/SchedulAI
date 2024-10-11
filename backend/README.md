# AI-Powered Task Scheduling App Backend

This is the backend for the AI-Powered Task Scheduling application, built with Node.js, Express, and TypeScript.

## Prerequisites

- Node.js (v14 or later recommended)
- npm (v6 or later)
- PostgreSQL

## Setup

1. Clone the repository
2. Navigate to the backend directory
3. Install dependencies:

   ```bash
   npm install
   ```

4. Create a `.env` file in the root of the backend directory with the following content:

   ```text
   PORT=3000
   DATABASE_URL=postgresql://username:password@localhost:5432/database_name
   ```

   Replace `username`, `password`, and `database_name` with your PostgreSQL credentials.

## Running the Server

To start the server in development mode:

```bash
npm run dev
```

For production:

```bash
npm run build
npm start
```

## Project Structure

- `src/server.ts`: Main application entry point
- `src/models/`: Database models
- `src/config/`: Configuration files, including database setup
- `src/middleware/`: Express middleware
- `src/utils/`: Utility functions, including logger

## Available Scripts

- `npm run dev`: Starts the server in development mode
- `npm run build`: Compiles TypeScript to JavaScript
- `npm start`: Starts the server in production mode
- `npm run lint`: Runs ESLint
- `npm run format`: Runs Prettier

## API Endpoints

- `GET /health`: Health check endpoint

More endpoints will be added as the project develops.

## Contributing

Please refer to the main project README for contribution guidelines.

## License

[MIT License](LICENSE)
