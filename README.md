# Cypress QA Automation Portfolio

![Cypress Tests](https://github.com/PixelA/cypress-qa-portfolio/actions/workflows/cypress.yml/badge.svg)

Cypress test suite demonstrating UI, API, and combined UI + API testing patterns, run automatically in GitHub Actions on every push.

## What's covered

| Spec | What it tests |
|---|---|
| `api_test.cy.js` | Public REST API (JSONPlaceholder): GET and POST requests, status codes, response body validation |
| `form_validation_test.cy.js` | Negative input scenarios: required fields, invalid formats, error messages |
| `portfolio_ui_test.cy.js` | UI navigation and element validation |
| `ui_api_combined_test.cy.js` | UI flows with network intercepts (`cy.intercept`) to verify the API calls behind the UI |

**In progress:** token-based authentication flow test

## Stack

Cypress · JavaScript · GitHub Actions

## Run locally

```bash
npm install
npx cypress run
```

Run specific specs:

```bash
npx cypress run --spec "cypress/e2e/api_test.cy.js,cypress/e2e/form_validation_test.cy.js"
```

## About

Built by Asherlee Levy, QA Automation Engineer. [LinkedIn](https://www.linkedin.com/in/asherleelevy)
