# 🧪 E2E Testing Project

Automated end-to-end testing suite using **Cypress 13** with continuous integration via **GitHub Actions**.

---
This project automates browser testing for login, signup, and checkout scenarios as part of the E2E testing coursework.


## Stack
- Cypress 13, Chrome headed/headless
- GitHub Actions CI

## Getting Started
1. `npm install`
2. Set `baseUrl` in `cypress.config.js`
3. `npm run cy:open` (interactive) or `npm test` (CI mode)

## Structure
- `cypress/e2e` — specs
- `cypress/support/commands.js` — custom commands
- `cypress/fixtures` — test data
- `.github/workflows/cypress.yml` — CI pipeline
- `testCases.md` — Exploratory notes + TS/TC

## Jira Workflow (screenshots required)
1. Create a Scrum project.
2. For each TC in `testCases.md`, create an issue (type: Task or Test).
3. Screenshot Backlog with all TC.
4. Create Sprint → move all TC into Sprint → screenshot Sprint backlog.
5. Start Sprint (do not complete) → screenshot Sprint board.

## Collaborators
Invite **Dailius** as a collaborator on GitHub (Settings → Collaborators).

## Scripts
- `npm run cy:open` — open Cypress
- `npm test` / `npm run cy:run` — headless run

## Conventions
- One scenario per spec file.
- Each `it()` is **one** test case.
- Use custom commands for repetitive UI flows (login, addToCart, checkout).
- Hooks (`beforeEach`) in every spec.
