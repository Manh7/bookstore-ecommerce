# Bookstore E-commerce

A full-stack e-commerce application for selling books and stationery.

## Project goals

- Build a complete portfolio project for Java Backend or Full-stack positions.
- Practice a professional software development workflow.
- Create a foundation for a future graduation project.
- Deploy a working application that recruiters can access.

## Technology stack

### Backend

- Java 21
- Spring Boot 3.5.x
- Maven
- Spring Data JPA
- Spring Security
- MySQL 8.4
- Flyway
- JUnit 5
- Mockito
- Testcontainers

### Frontend

- Angular 19.2
- Node.js 22
- TypeScript
- HTML
- SCSS
- RxJS

### Development and deployment

- Git and GitHub
- Docker and Docker Compose
- GitHub Actions

## Repository structure

```text
bookstore-ecommerce/
├── backend/          # Spring Boot API
├── frontend/         # Angular application
├── infra/            # Infrastructure as code
├── docs/             # Documentation
├── .github/          # GitHub workflows
├── compose.yaml      # Docker Compose configuration
└── README.md         # This file
```

## Getting Started

### Prerequisites

**Backend:**
- Java 21 or higher
- Maven 3.6 or higher
- MySQL 8.4 (or use Docker)

**Frontend:**
- Node.js 22.x or higher
- npm 10.x or higher

### Installation

#### Backend Setup

1. Navigate to the backend directory:
```bash
cd backend
```

2. Build the project:
```bash
./mvnw clean install
```

3. Run the application:
```bash
./mvnw spring-boot:run
```

The backend API will be available at `http://localhost:8080`.

For detailed backend setup and configuration, see [backend/README.md](backend/README.md).

#### Frontend Setup

1. Navigate to the frontend directory:
```bash
cd frontend
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm start
```

The frontend application will be available at `http://localhost:4200`.

For detailed frontend setup and configuration, see [frontend/README.md](frontend/README.md).

### Running with Docker Compose

To run the entire stack using Docker Compose:

```bash
docker compose up
```

This will start all services defined in `compose.yaml`.

## Development Workflow

1. Create a feature branch from `main`
2. Make your changes and commit them
3. Push your branch and create a pull request
4. After review and approval, merge to `main`

## Contributing

This is a personal portfolio project, but suggestions and feedback are welcome.