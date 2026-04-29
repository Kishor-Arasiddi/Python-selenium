# Python Selenium Automation

A comprehensive Selenium WebDriver automation framework in **Python** covering a wide range of browser automation techniques — from basic interactions to advanced patterns like data-driven testing, headless execution, and synchronization strategies.

## 📁 Project Structure

```
├── .idea/                        # PyCharm / IntelliJ project configuration
├── CookieHandle/                 # Cookie management — reading, writing, and deleting browser cookies
├── Data/                         # Test data files used across the framework
├── Datadriven_Testing/           # Data-driven tests using external data sources (Excel, CSV, etc.)
├── Demo/                         # Demo scripts and introductory examples
├── Handlings/                    # Handling UI scenarios (alerts, dropdowns, checkboxes, etc.)
├── Headless_mode/                # Running browser automation in headless (no-UI) mode
├── ScreenShot_program/           # Capturing screenshots during test execution
├── Synchronization_programs/     # Implicit/explicit waits and expected conditions
├── access_in_xpath/              # XPath locator strategies and access patterns
├── actionchain_programs/         # ActionChains API — hover, drag-and-drop, right-click, etc.
├── drivers/                      # WebDriver binaries (chromedriver, geckodriver, etc.)
├── file_Download/                # Automating file download scenarios
├── frame_programs/               # Handling iframes and nested frames
├── javascriptExecutor_programs/  # Executing JavaScript via execute_script()
├── popup_programs/               # Handling browser popups, alerts, and confirmation dialogs
├── webdriver_programs/           # Core WebDriver setup and fundamental browser interactions
└── README.md
```

## 🚀 Getting Started

### Prerequisites

- Python 3.7+
- pip
- Chrome / Firefox browser installed
- Matching WebDriver binary in the `drivers/` folder (or use `webdriver-manager`)

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd <repository-name>
   ```

2. **Install dependencies**
   ```bash
   pip install selenium
   pip install webdriver-manager   # optional but recommended
   pip install openpyxl             # for data-driven Excel tests
   ```

3. **Configure WebDriver** — either place the driver binary in `drivers/` or use `webdriver-manager`:
   ```python
   from selenium import webdriver
   from webdriver_manager.chrome import ChromeDriverManager

   driver = webdriver.Chrome(ChromeDriverManager().install())
   ```

4. **Run any script**
   ```bash
   python webdriver_programs/your_script.py
   ```

## 📦 Module Overview

### `webdriver_programs`
Core WebDriver setup — launching browsers, navigating URLs, locating elements, and performing basic interactions like `click()` and `send_keys()`.

### `Handlings`
Covers handling of common UI components — alerts, `Select` dropdowns, checkboxes, and radio buttons.

### `Synchronization_programs`
Demonstrates `implicitly_wait`, `WebDriverWait` with `expected_conditions`, and custom polling strategies to handle dynamic pages.

### `actionchain_programs`
Uses Selenium's `ActionChains` class for complex mouse and keyboard interactions — hover, double-click, drag-and-drop, and key combinations.

### `javascriptExecutor_programs`
Executes JavaScript in the browser using `driver.execute_script()` — useful for scrolling, clicking hidden elements, and reading DOM properties.

### `frame_programs`
Switching into and out of iframes and nested frames using `driver.switch_to.frame()`.

### `popup_programs`
Handling browser-level popups, JavaScript alerts, confirm dialogs, and prompts via `driver.switch_to.alert`.

### `CookieHandle`
Adding, retrieving, and deleting cookies using `driver.add_cookie()`, `driver.get_cookies()`, and `driver.delete_cookie()`.

### `Headless_mode`
Running Chrome or Firefox in headless mode using `ChromeOptions` — ideal for CI/CD pipelines.

```python
from selenium.webdriver.chrome.options import Options

options = Options()
options.add_argument("--headless")
driver = webdriver.Chrome(options=options)
```

### `ScreenShot_program`
Capturing screenshots using `driver.save_screenshot()` and `element.screenshot()`.

### `file_Download`
Configuring Chrome/Firefox preferences to handle automatic file downloads without dialog prompts.

### `access_in_xpath`
XPath expressions in Python Selenium — absolute vs relative XPath, text nodes, attributes, axes, and chained predicates.

### `Datadriven_Testing`
Parameterizing tests with data from external sources such as Excel (`openpyxl`) or CSV files, often combined with `pytest` parametrize.

## 🛠️ Technologies Used

- **Selenium WebDriver** — browser automation
- **Python 3** — primary language
- **pytest** — test execution and parameterization
- **openpyxl** — Excel data handling
- **webdriver-manager** — automatic driver management
- **ChromeDriver / GeckoDriver** — browser drivers

## 📌 Tips

- Always match your ChromeDriver version to your installed Chrome browser version.
- Prefer `WebDriverWait` + `expected_conditions` over `time.sleep()` for stable tests.
- Use headless mode for running tests in CI/CD environments (GitHub Actions, Jenkins, etc.).
- Store locators separately (Page Object Model) for larger projects.

## 📄 License

This project is intended for educational and practice purposes.
