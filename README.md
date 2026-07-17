# React 2 Demo

A small React application originally created with Create React App. The repository is retained as a compact example project and is being prepared for safer, reproducible maintenance.

## Technology stack

- React 17
- Create React App 4
- JavaScript
- React Testing Library

## Local development

Requirements:

- Node.js 20 LTS
- npm 10 or newer

Install dependencies and start the development server:

```bash
npm ci
npm start
```

The application is available at `http://localhost:3000`.

## Production build

```bash
npm ci
npm run build
```

The optimized output is written to the `build/` directory.

## Tests

Run the test suite once in CI mode:

```bash
npm test -- --watchAll=false
```

## Security and maintenance

GitHub Actions verifies installation, tests, the production build and the production dependency audit on pull requests and pushes to the default branch. Dependabot checks npm and GitHub Actions dependencies weekly.

The project currently uses the legacy Create React App toolchain. A future major modernization should migrate the application to Vite and a currently supported React version in a dedicated pull request, because that change can affect runtime behavior and the lockfile substantially.

## Repository structure

```text
public/       static assets
src/          application source and tests
package.json  scripts and dependencies
```
