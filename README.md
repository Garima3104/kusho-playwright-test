# Playwright Test Automation Project

This project contains automated tests using Playwright with TypeScript.

## Prerequisites

Before running the tests, make sure you have the following installed:

- Node.js 14 or higher
- npm (Node package manager)
- TypeScript

## Installation

1. Clone the repository:

```bash
git clone <your-repository-url>
cd <project-directory>
```

1. Install dependencies:

```bash
npm install
```

1. Install Playwright browsers:

```bash
npx playwright install
```

## Running Tests

1. Run all tests:

```bash
npx playwright test
```

or

```bash
npx playwright test --ui
```

1. Run specific test file:

```bash
npx playwright test tests/test_specific.ts
```

1. Run tests in headed mode:

```bash
npx playwright test --headed
```

1. Run tests with specific browser:

```bash
npx playwright test --project=chromium  # or firefox, webkit
```

1. Run tests in parallel:

```bash
npx playwright test --workers=auto
```

## Configuration

- Default browser: Chromium
- Headless mode: Enabled by default
- Viewport size: 1280x720
- Test timeout: 30 seconds

## Debugging

1. Run tests in debug mode:

```bash
npx playwright test --debug
```

1. Use Playwright Inspector:

```bash
PWDEBUG=1 npx playwright test
```

## Reporting

Generate HTML report:

```bash
npx playwright show-report
```

## Common Issues

1. If you encounter browser launch issues:

```bash
npx playwright install
```

1. For permission issues on Linux:

```bash
sudo apt-get install libgbm1
```
