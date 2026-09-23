# Angular Template

A modern, opinionated Angular starter used as the base for new applications. Standalone
components, zoneless change detection, and Tailwind CSS are configured out of the box, along
with linting, formatting, and commit hooks.

## Stack

- **Angular 22** — standalone components, signals, zoneless change detection, new `@for`/`@if`
  control flow.
- **Tailwind CSS 4** — CSS-first config via `@import 'tailwindcss'` in [src/styles.css](src/styles.css);
  no `tailwind.config.js` needed. Customize design tokens with an `@theme` block in that file.
- **TypeScript** — `strict` mode and Angular's `strictTemplates` enabled.
- **ESLint + Prettier** — `eslint.config.js` (flat config) with `angular-eslint`;
  `prettier-plugin-tailwindcss` auto-sorts utility classes.
- **Vitest** — Angular's built-in unit test runner.
- **Husky + lint-staged + commitlint** — staged files are linted/formatted on commit; commit
  messages are checked against [Conventional Commits](https://www.conventionalcommits.org/).
- **Path alias** — `@app/*` resolves to `src/app/*` (see [tsconfig.json](tsconfig.json)).

## Prerequisites

- Node.js 20+ and npm

## Getting started

```bash
npm install
npm start
```

Open `http://localhost:4200/`. The app reloads automatically as you edit files.

## Scripts

| Script                 | Description                               |
| ---------------------- | ----------------------------------------- |
| `npm start`            | Run the dev server (`ng serve`).          |
| `npm run build`        | Production build, output to `dist/`.      |
| `npm run watch`        | Development build in watch mode.          |
| `npm test`             | Run unit tests with Vitest.               |
| `npm run lint`         | Lint `.ts`/`.html` files under `src/`.    |
| `npm run format`       | Format `src/` with Prettier.              |
| `npm run format:check` | Check formatting without writing changes. |

## Using this as a template

1. Update the project name in [package.json](package.json) and the `projects` key in
   [angular.json](angular.json).
2. Replace the placeholder markup in [src/app/app.html](src/app/app.html).
3. Start building — routes live in [src/app/app.routes.ts](src/app/app.routes.ts), app-wide
   providers in [src/app/app.config.ts](src/app/app.config.ts).

## Additional resources

- [Angular CLI reference](https://angular.dev/tools/cli)
- [Tailwind CSS docs](https://tailwindcss.com/docs)
