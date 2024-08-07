# Learning cards app

[![codecov](https://codecov.io/gh/wtchnm/Vitamin/branch/main/graph/badge.svg?token=H9BBAKGYI0)](https://codecov.io/gh/wtchnm/Vitamin) ![Test workflow](https://github.com/wtchnm/Vitamin/actions/workflows/test.yml/badge.svg) ![CodeQL workflow](https://github.com/wtchnm/Vitamin/actions/workflows/codeql-analysis.yml/badge.svg) [![Vitamin](https://img.shields.io/endpoint?url=https://dashboard.cypress.io/badge/simple/etow1b&style=flat&logo=cypress)](https://dashboard.cypress.io/projects/etow1b/runs) [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier) [![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)

## Tech stack

- [Vite](https://vitejs.dev) with [React](https://reactjs.org), [TypeScript](https://www.typescriptlang.org) and [absolute imports](https://github.com/aleclarson/vite-tsconfig-paths).
- [Tailwind CSS v3](https://tailwindcss.com) with a [basic reset for form styles](https://github.com/tailwindlabs/tailwindcss-forms) and a [Prettier plugin](https://github.com/tailwindlabs/prettier-plugin-tailwindcss) that automatically sorts classes.
- Use [ESLint](https://eslint.org), [stylelint](https://stylelint.io) and [Prettier](https://prettier.io) on VSCode and before you commit with [Husky](https://github.com/typicode/husky) and [lint-staged](https://github.com/okonet/lint-staged).
- [PWA](https://github.com/antfu/vite-plugin-pwa) with [17/17 Lighthouse score](https://web.dev/pwa-checklist/).
- Write unit and integration tests with [Vitest](https://vitest.dev/) and [Testing Library](https://testing-library.com/).
- Write e2e tests with [Cypress](https://www.cypress.io).

## Getting started

Install the dependencies:

```
pnpm install
```

## Scripts

- `pnpm dev` - start a development server with hot reload.
- `pnpm build` - build for production. The generated files will be on the `dist` folder.
- `pnpm preview` - locally preview the production build.
- `pnpm test` - run unit and integration tests related to changed files based on git.
- `pnpm test:ci` - run all unit and integration tests in CI mode.
- `pnpm test:e2e` - run all e2e tests with the Cypress Test Runner.
- `pnpm test:e2e:headless` - run all e2e tests headlessly.
- `pnpm format` - format all files with Prettier.
- `pnpm lint` - runs TypeScript, ESLint and Stylelint.
- `pnpm validate` - runs `lint`, `test:ci` and `test:e2e:ci`.
