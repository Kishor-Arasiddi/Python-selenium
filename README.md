# Python Selenium Automation Examples

This repository contains a comprehensive collection of Python Selenium scripts demonstrating various web automation concepts, techniques, and best practices. It serves as a practical guide and reference for handling common scenarios encountered in UI test automation.

## 📁 Repository Structure

The project is organized into modular directories based on specific Selenium features and testing strategies:

* **`access_in_xpath/`**: Advanced techniques for locating web elements using complex XPath axes and functions.
* **`actionchain_programs/`**: Scripts demonstrating mouse and keyboard interactions (e.g., drag and drop, hover, right-click) using the `ActionChains` class.
* **`CookieHandle/`**: Examples of how to add, retrieve, and delete browser cookies during a testing session.
* **`Data/`**: Directory dedicated to storing external test data files (e.g., CSV, Excel, or JSON).
* **`Datadriven_Testing/`**: Implementations of Data-Driven Testing (DDT) approaches, reading test data from external sources to run multiple test iterations.
* **`Demo/`**: Basic demonstration scripts outlining standard automation workflows.
* **`drivers/`**: Contains the necessary browser executables (like ChromeDriver, GeckoDriver) required by Selenium WebDriver.
* **`file_Download/`**: Automation strategies for handling and verifying file downloads from web applications.
* **`frame_programs/`**: Techniques for switching contexts to interact with elements inside `iframe` and `frame` tags.
* **`Handlings/`**: Various element handling methods (e.g., dropdowns, checkboxes, dynamic web elements).
* **`Headless_mode/`**: Configurations for running browser tests in the background without a graphical user interface (useful for CI/CD pipelines).
* **`javascriptExecutor_programs/`**: Scripts that execute raw JavaScript commands directly within the browser context to perform actions or retrieve values.
* **`popup_programs/`**: Examples of managing JavaScript alerts, confirmation dialogs, and browser-native pop-ups.
* **`ScreenShot_program/`**: Utility scripts for capturing and saving screenshots of the browser window during test execution or upon failure.
* **`Synchronization_programs/`**: Demonstrations of different wait strategies (Implicit Waits, Explicit Waits, and Fluent Waits) to handle dynamic content loading.
* **`webdriver_programs/`**: Core WebDriver initialization, navigation, and basic browser interaction scripts.

## 🛠️ Prerequisites

To run these scripts, ensure you have the following installed on your machine:

* **Python 3.x**: [Download Python](https://www.python.org/downloads/)
* **Selenium WebDriver**: Python bindings for Selenium.

## 🚀 Setup and Installation

1. **Clone the repository:**
   
```bash
   git clone [https://github.com/Kishor-Arasiddi/Python-selenium.git](https://github.com/Kishor-Arasiddi/Python-selenium.git)
   cd Python-selenium
```
2. **Install the required dependencies:**
It is recommended to use a virtual environment.

```
pip install selenium

```
3. **Configure WebDrivers:**

Ensure that the appropriate browser drivers are present in the drivers/ directory or added to your system's PATH. Alternatively, you can use webdriver-manager to handle this automatically in your scripts.

## Usage:

Navigate to the specific directory of the concept you want to explore and run the Python script directly. For example:

```
cd actionchain_programs
python <script_name>.py
```

