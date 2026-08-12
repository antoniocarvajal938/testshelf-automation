# TestShelf Automation 🧪

Automated end-to-end testing framework for the **TestShelf** e-commerce
application.

This project is built with **Node.js, TypeScript and Playwright**,
following a maintainable and scalable **Page Object Model (POM)**
architecture.

The main goal is to provide a realistic environment for practicing and
demonstrating **QA Automation skills**, from test planning and test case
design to automated execution, reporting and CI/CD integration.

------------------------------------------------------------------------

## 🎯 Project Goals

The project is designed to practice and demonstrate:

-   End-to-end test automation
-   Test planning and test case design
-   Page Object Model (POM) architecture
-   Maintainable and reusable test code
-   Robust element identification and locators
-   Test data management
-   Positive and negative test scenarios
-   Functional testing
-   Regression testing
-   Cross-browser testing
-   Automated test reporting
-   CI/CD integration
-   GitHub Actions
-   QA Automation best practices

------------------------------------------------------------------------

## 🛠️ Tech Stack

  Technology       Purpose
  ---------------- ------------------------------------
  Node.js          Runtime and dependency management
  TypeScript       Programming language
  Playwright       End-to-end test automation
  Git              Version control
  GitHub           Source code repository
  GitHub Actions   CI/CD and automated test execution

------------------------------------------------------------------------

## 🌐 Application Under Test

The tests in this repository target **TestShelf**, an e-commerce web
application created specifically to provide a realistic environment for
QA Automation practice.

### Application

**Live Demo:**\
YOUR_TESTSHELF_URL

### Frontend Repository

**TestShelf Repository:**\
https://github.com/antoniocarvajal938/testshelf-ecommerce-qa

------------------------------------------------------------------------

## 🏗️ Project Architecture

The automation framework follows a **Page Object Model (POM)**
architecture.

``` text
testshelf-automation/
│
├── data/
│   └── Test data and test-related information
│
├── pages/
│   └── Page Object classes
│
├── tests/
│   └── Automated test specifications
│
├── utils/
│   └── Reusable utilities and helper functions
│
├── .env.example
├── .gitignore
├── package.json
├── package-lock.json
├── playwright.config.ts
└── README.md
```

### `tests/`

Contains the automated test specifications.

Tests are organized according to the application's functional areas and
are responsible for validating expected user behaviour.

### `pages/`

Contains the Page Object classes used to encapsulate page-specific
locators and interactions.

This separation helps reduce code duplication and makes the test suite
easier to maintain when the application changes.

### `data/`

Contains reusable test data required by the automated tests.

Examples may include:

-   User credentials
-   Product information
-   Expected values
-   Test scenarios

### `utils/`

Contains reusable helper functions and utilities that are not specific
to a single page.

------------------------------------------------------------------------

## ⚙️ Installation

Clone the repository:

``` bash
git clone git@github.com:antoniocarvajal938/testshelf-automation.git
```

Navigate to the project:

``` bash
cd testshelf-automation
```

Install dependencies:

``` bash
npm install
```

Install Playwright browsers:

``` bash
npx playwright install
```

------------------------------------------------------------------------

## 🔐 Environment Configuration

The application URL is configured using environment variables.

Create a `.env` file in the project root:

``` env
BASE_URL=YOUR_TESTSHELF_URL
```

The `.env` file is intentionally excluded from version control.

A `.env.example` file is provided as a reference for the required
environment variables.

------------------------------------------------------------------------

## ▶️ Running Tests

Run the complete test suite:

``` bash
npx playwright test
```

Run tests using Playwright UI Mode:

``` bash
npx playwright test --ui
```

Run a specific test file:

``` bash
npx playwright test tests/<test-file>.spec.ts
```

Run tests in a specific browser:

``` bash
npx playwright test --project=chromium
```

------------------------------------------------------------------------

## 🌍 Cross-Browser Testing

The framework is configured to support testing across multiple browser
engines:

-   Chromium
-   Firefox
-   WebKit

Additional browser and mobile configurations can be enabled through
`playwright.config.ts`.

------------------------------------------------------------------------

## 📊 Test Reports

Playwright HTML reports are generated after test execution.

To open the latest report:

``` bash
npx playwright show-report
```

Reports can provide information such as:

-   Passed tests
-   Failed tests
-   Execution time
-   Screenshots
-   Traces
-   Test steps

------------------------------------------------------------------------

## 🔄 CI/CD

The project integrates with **GitHub Actions** to automatically execute
the Playwright test suite.

The workflow is triggered by:

-   Pushes to the `main` branch
-   Pull Requests targeting the `main` branch

The CI pipeline:

1.  Checks out the repository
2.  Installs Node.js
3.  Installs project dependencies
4.  Installs Playwright browsers
5.  Executes the automated test suite
6.  Uploads the Playwright report as a workflow artifact

------------------------------------------------------------------------

## 🧪 Testing Strategy

The test strategy is based on the functional behaviour and risk of the
application.

The test plan covers areas such as:

-   Home
-   Navigation
-   Product catalogue
-   Product details
-   Authentication
-   Shopping cart
-   Checkout
-   Contact functionality
-   Responsive behaviour
-   Validation and error scenarios

Tests are prioritized according to:

-   Business impact
-   Risk
-   User impact
-   Functional criticality
-   Suitability for automation

------------------------------------------------------------------------

## 📋 Test Coverage

Test coverage will be progressively expanded as the project evolves.

  Functional Area        Status
  ---------------------- ----------------
  Home                   🚧 In progress
  Navigation             🚧 In progress
  Products               🚧 In progress
  Product Details        🚧 In progress
  Login                  🚧 In progress
  Cart                   🚧 In progress
  Checkout               🚧 In progress
  Contact                🚧 In progress
  Responsive Behaviour   🚧 In progress

------------------------------------------------------------------------

## 📈 Future Improvements

Potential future improvements include:

-   Expanded test coverage
-   Advanced Playwright fixtures
-   Improved test data management
-   Authentication state management
-   Environment-based configuration
-   Parallel execution optimization
-   Enhanced reporting
-   CI/CD improvements
-   Integration with external test management tools
-   API testing
-   Performance testing

------------------------------------------------------------------------

## 👨‍💻 Project Status

> 🚧 **This project is currently under development.**

The framework, test plan and automated test suite are being
progressively built as part of a practical **QA Automation project**
focused on applying professional testing practices with **Playwright and
TypeScript**.

The final objective is to provide a complete, maintainable and realistic
automation framework that can be used both as a **learning resource and
portfolio project**.

------------------------------------------------------------------------

## 📄 License

This project is intended for educational and portfolio purposes.
