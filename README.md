# ui_test_automation_playwright

A modern UI test automation framework built with Playwright for end-to-end testing.

## GitHub Copilot prompt used to create this repository's content

```
Generate a Playwright test automation framework in TypeScript. The framework should include:

1.  **Project Structure:**
    *   A `tests` directory for test files.
    *   A `pages` directory for Page Object Model (POM) files.
    *   A `fixtures` directory for custom test fixtures.
    *   A `utils` directory for helper functions.
    *   A `playwright.config.ts` file with basic configurations (e.g., browser setup for Chromium, Firefox, WebKit, headless mode, base URL, retries, reporting).
```

## 🚀 Getting Started

### Prerequisites

- Node.js (version 18 or higher)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/drcolburn/ui_test_automation_playwright.git
cd ui_test_automation_playwright
```

2. Install dependencies:
```bash
npm install
```

3. Install Playwright browsers:
```bash
npx playwright install
```

## 📖 Usage

### Running Tests

Run all tests:
```bash
npm test
```

Run tests in headed mode (see browser):
```bash
npm run test:headed
```

Run tests in debug mode:
```bash
npm run test:debug
```

Run tests in UI mode (interactive):
```bash
npm run test:ui
```

View test report:
```bash
npm run test:report
```

### Writing Tests

Tests are located in the `tests/` directory. Example test structure:

```typescript
import { test, expect } from '@playwright/test';

test.describe('Feature Name', () => {
  test('test description', async ({ page }) => {
    await page.goto('https://example.com');
    // Your test code here
  });
});
```

## 📁 Project Structure

```
ui_test_automation_playwright/
├── tests/              # Test files
├── playwright.config.ts # Playwright configuration
├── package.json        # Project dependencies and scripts
└── README.md          # This file
```

## 🛠️ Configuration

The Playwright configuration is in `playwright.config.ts`. You can customize:

- Test directory
- Browser settings
- Parallel execution
- Retry logic
- Reporting options
- And more...

## 📚 Resources

- [Playwright Documentation](https://playwright.dev/)
- [Playwright API Reference](https://playwright.dev/docs/api/class-playwright)
- [Best Practices](https://playwright.dev/docs/best-practices)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the ISC License.
