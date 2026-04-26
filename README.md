# BankBot-Selenium-Java-Test-Automation-Framework
BankBot – Selenium-Java Test Automation Framework is a scalable automation framework built using Selenium WebDriver, Java, and TestNG to automate end-to-end testing of an online banking application.  The framework follows the Page Object Model (POM) design pattern to ensure modularity, reusability, and maintainability.


# 🏦 BankBot – Selenium Java Automation Framework

## 📌 Overview

BankBot is a Selenium-based test automation framework built using **Java, Selenium WebDriver, and TestNG** to automate testing of an online banking application.

The framework follows the **Page Object Model (POM)** design pattern to ensure clean structure, reusability, and maintainability. It automates end-to-end workflows such as login, customer creation, account handling, and fund transfers.

This project is designed to simulate a **real-world automation framework used in industry**, not just standalone scripts.

---

## 🚀 Tech Stack

* Java
* Selenium WebDriver
* TestNG
* Maven
* WebDriverManager
* ExtentReports

---

## 🌐 Application Under Test

https://demo.guru99.com/V4/index.php

---

## 📂 Project Structure

```
src/main/java
│
├── base        → Base classes (BasePage, BaseTest)
├── pages       → Page Object classes (LoginPage, NewCustomerPage, etc.)
├── utils       → Utilities (ConfigReader, Screenshot, Waits)
│
src/test/java
│
├── tests       → Test classes
│
resources
│
├── config.properties
├── testng.xml
```

---

## ✅ Features

* Page Object Model (POM) design
* Data-driven testing using TestNG DataProvider
* Explicit waits using WebDriverWait
* Screenshot capture on test failure
* ExtentReports for HTML reporting
* Config-driven execution (browser, URL, timeout)

---

## 🧪 Test Coverage

### 🔐 Authentication Module

* Valid login
* Invalid login
* Logout verification
* Blank field validation

### 👤 Customer Management

* Create new customer
* Verify customer ID generation
* Validate success message
* Duplicate email validation

### 💳 Account Management

* Create new account
* Edit account details
* Invalid customer ID validation

### 💸 Fund Transfer

* Transfer funds between accounts
* Verify updated balance
* Invalid transfer validation

### ⚠️ Form Validation

* Empty field validation
* Invalid input handling
* Date validation (DOB constraints)

---

## ⚙️ Configuration

All configurable values are stored in:

```
config.properties
```

Example:

```
browser=chrome
baseUrl=https://demo.guru99.com/V4/index.php
timeout=10
```

---

## ▶️ How to Run Tests

### Using Maven:

```
mvn test
```

### Using TestNG:

* Right click on `testng.xml` → Run

---

## 📊 Reports

* Extent Report generated at:

```
/test-output/ExtentReport.html
```

* Screenshots on failure:

```
/screenshots/
```

---

## 🧠 Key Design Principles

* No hardcoded values (everything from config)
* No WebDriver calls in test classes
* Reusable methods in BasePage
* Clear separation between Page, Test, and Utility layers

---

## 👨‍💻 Author

Manoj
