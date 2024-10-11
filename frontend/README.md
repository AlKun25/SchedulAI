# AI-Powered Task Scheduling App

## Project Overview

This project is an AI-powered task scheduling web application built with Vue.js and TypeScript. It integrates with Google Calendar and utilizes LLM-based scheduling algorithms to provide efficient task management and scheduling capabilities.

## Features

- User authentication
- Google Calendar integration
- AI-driven task scheduling
- Responsive web interface
- Enhanced image-based event and task creation

## Technology Stack

- Frontend: Vue.js 3 with TypeScript
- State Management: Vuex
- Routing: Vue Router
- API Calls: Axios
- Testing: Jest (Unit), Cypress (E2E)
- Linting: ESLint
- Formatting: Prettier
- Containerization: Docker

## Project Structure

```
.
├── public/                 # Public assets
├── src/                    # Source files
│   ├── assets/             # Static assets
│   ├── components/         # Vue components
│   ├── router/             # Vue Router configuration
│   ├── store/              # Vuex store
│   ├── views/              # Vue views
│   ├── App.vue             # Main app component
│   └── main.ts             # App entry point
├── tests/                  # Test files
│   ├── e2e/                # End-to-end tests (Cypress)
│   └── unit/               # Unit tests (Jest)
├── Dockerfile              # Docker configuration
├── babel.config.js         # Babel configuration
├── cypress.json            # Cypress configuration
├── jest.config.js          # Jest configuration
├── package.json            # Project dependencies and scripts
├── tsconfig.json           # TypeScript configuration
└── vue.config.js           # Vue CLI configuration
```

## Getting Started

### Prerequisites

- Node.js (v14 or later)
- npm (v6 or later)

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

### Development

To run the development server:

```bash
npm run serve
```

The application will be available at `http://localhost:8080`.

### Building for Production

To create a production build:

```bash
npm run build
```

The built files will be in the `dist/` directory.

### Docker

To build and run the Docker container:

```bash
docker build -t ai-task-scheduler .
docker run -p 8080:80 ai-task-scheduler
```

## Testing

### Unit Tests

Run unit tests with Jest:

```bash
npm run test:unit
```

### End-to-End Tests

Run e2e tests with Cypress:

```bash
npm run test:e2e
```

## Linting

To lint and fix files:

```bash
npm run lint
```

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

- [Vue.js](https://vuejs.org/)
- [TypeScript](https://www.typescriptlang.org/)
- [Google Calendar API](https://developers.google.com/calendar)
