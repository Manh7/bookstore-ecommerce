# Quick Start Guide

## Prerequisites Check

Before starting, verify your environment:

```bash
node --version  # Should be 22.x or higher
npm --version   # Should be 10.x or higher
```

## Installation & Setup (5 minutes)

1. **Install dependencies:**
   ```bash
   npm install
   ```

2. **Start development server:**
   ```bash
   npm start
   ```

3. **Open your browser:**
   Navigate to `http://localhost:4200`

That's it! The application is now running.

## Common Commands

| Command | Description |
|---------|-------------|
| `npm start` | Start development server on port 4200 |
| `npm run build` | Create production build |
| `npm test` | Run unit tests |
| `npm run watch` | Build in watch mode |
| `ng generate component <name>` | Generate a new component |
| `ng generate service <name>` | Generate a new service |

## Project Configuration

- **Framework:** Angular 19.2
- **Node Version:** 22.x
- **Styling:** SCSS
- **Components:** Standalone (no NgModules)
- **Routing:** Enabled
- **SSR:** Enabled (Server-Side Rendering)

## Environment Configuration

The application uses environment files for configuration:

- `src/environments/environment.ts` - Development configuration
- `src/environments/environment.prod.ts` - Production configuration

**Backend API URL:**
- Development: `http://localhost:8080/api`
- Production: `/api` (relative path)

## Next Steps

1. **Create your first component:**
   ```bash
   ng generate component components/book-list
   ```

2. **Create your first service:**
   ```bash
   ng generate service services/book
   ```

3. **Add a route:**
   Edit `src/app/app.routes.ts`

## Troubleshooting

### Port 4200 already in use
```bash
# Kill the process using port 4200
# Windows:
netstat -ano | findstr :4200
taskkill /PID <PID> /F

# Or use a different port:
ng serve --port 4300
```

### Build errors after updating dependencies
```bash
# Clear cache and reinstall
rm -rf node_modules package-lock.json
npm install
```

### Angular CLI not found
```bash
# Install Angular CLI globally
npm install -g @angular/cli@19.2
```

## Development Tips

1. **Hot Module Replacement:** Changes to `.ts`, `.html`, and `.scss` files automatically reload the browser
2. **TypeScript Strict Mode:** Enabled - provides better type safety
3. **Lazy Loading:** Use route-based code splitting for better performance
4. **Standalone Components:** Import dependencies directly in component metadata

## Need Help?

- [Angular Documentation](https://angular.dev)
- [Angular CLI Documentation](https://angular.dev/tools/cli)
- [TypeScript Handbook](https://www.typescriptlang.org/docs/)
