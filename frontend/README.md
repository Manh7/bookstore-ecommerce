# Bookstore E-Commerce - Frontend

This is the frontend application for the Bookstore E-Commerce platform, built with Angular 19.2.

## Prerequisites

- Node.js 22.x or higher
- npm 10.x or higher

## Technology Stack

- **Framework**: Angular 19.2
- **Styling**: SCSS
- **Architecture**: Standalone Components
- **Routing**: Angular Router
- **Server-Side Rendering**: Angular SSR

## Installation

1. Navigate to the frontend directory:
```bash
cd frontend
```

2. Install dependencies:
```bash
npm install
```

## Development

### Running the Development Server

Start the development server:
```bash
npm start
```
or
```bash
ng serve
```

The application will be available at `http://localhost:4200/`. The development server will automatically reload when you make changes to the source files.

### Building for Production

Build the application for production:
```bash
npm run build
```

The build artifacts will be stored in the `dist/frontend/` directory.

### Running Production Build

To run the server-side rendered application:
```bash
npm run serve:ssr:frontend
```

## Project Structure

```
frontend/
├── src/
│   ├── app/
│   │   ├── app.component.ts       # Root component
│   │   ├── app.component.html     # Root template
│   │   ├── app.component.scss     # Root styles
│   │   ├── app.config.ts          # Application configuration
│   │   └── app.routes.ts          # Routing configuration
│   ├── main.ts                    # Application entry point
│   ├── main.server.ts             # Server entry point
│   ├── server.ts                  # Express server
│   ├── index.html                 # Main HTML file
│   └── styles.scss                # Global styles
├── public/                        # Static assets
├── angular.json                   # Angular CLI configuration
├── package.json                   # Dependencies and scripts
└── tsconfig.json                  # TypeScript configuration
```

## Available Scripts

- `npm start` - Start the development server
- `npm run build` - Build the application for production
- `npm run watch` - Build in watch mode for development
- `npm test` - Run unit tests with Karma
- `npm run serve:ssr:frontend` - Serve the SSR application

## Configuration

### Angular Configuration
The project uses standalone components, which means:
- No `NgModule` declarations needed
- Components are self-contained with their dependencies
- Improved tree-shaking and bundle sizes

### Styling
- SCSS is configured as the default styling format
- Global styles are in `src/styles.scss`
- Component-specific styles use the `.scss` extension

### Routing
- Routing is enabled and configured in `src/app/app.routes.ts`
- The `<router-outlet>` is placed in the root component

## Integration with Backend

The frontend is designed to integrate with a Spring Boot backend. API endpoint configurations will be added as the backend services are developed.

### Future API Integration
- Base API URL configuration will be in environment files
- HTTP interceptors will handle authentication and error handling
- Services will be created to communicate with backend REST APIs

## Code Style and Best Practices

- Use Angular standalone components
- Follow Angular style guide
- Use TypeScript strict mode
- Write meaningful component and variable names
- Keep components focused and single-purpose

## Additional Resources

- [Angular Documentation](https://angular.dev)
- [Angular CLI Documentation](https://angular.dev/tools/cli)
- [TypeScript Documentation](https://www.typescriptlang.org/docs/)
