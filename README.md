# Selenium Web Automation – Mercari

## 📌 Project Overview

This is a web automation project developed using **Java, Selenium WebDriver, Maven, TestNG, and the Page Object Model (POM)**.

The project was created in **Eclipse** as part of a web automation assignment. It automates two scenarios on the Mercari application and generates execution reports using **ExtentReports**.

## 🛠️ Technologies Used

| Technology         | Purpose                           |
| ------------------ | --------------------------------- |
| Java               | Programming language              |
| Selenium WebDriver | Browser automation                |
| TestNG             | Test execution and assertions     |
| Maven              | Project and dependency management |
| Page Object Model  | Framework design                  |
| PageFactory        | Page object initialization        |
| ExtentReports      | Test execution reporting          |
| Eclipse            | Development environment           |

## 🏗️ Project Structure

```text
QA Assignment - Web/
│
├── drivers/
│   ├── chromedriver.exe
│   ├── geckodriver.exe
│   └── IEDriverServer.exe
│
├── src/
│   ├── main/
│   │   └── java/
│   │       └── pfPackage/
│   │           ├── base/
│   │           │   └── BasePage.java
│   │           │
│   │           ├── pages/
│   │           │   ├── ItemsDetailsPage.java
│   │           │   ├── MyPage.java
│   │           │   ├── PersonalInfoPage.java
│   │           │   ├── SearchedItemsPage.java
│   │           │   ├── ShippingAddressPage.java
│   │           │   ├── TimeLinePage.java
│   │           │   └── UpdateShippingPage.java
│   │           │
│   │           └── util/
│   │               ├── Constants.java
│   │               └── ExtentManager.java
│   │
│   └── test/
│       ├── java/
│       │   └── pfPack/
│       │       └── tests/
│       │           ├── MercariScenario01.java
│       │           ├── MercariScenario02.java
│       │           └── base/
│       │               └── BaseTest.java
│       │
│       └── resources/
│           └── testng.xml
│
├── reports/
├── screenshots/
├── test-output/
├── pom.xml
└── README.md
```

## 🧪 Test Scenarios

### Scenario 1

The first scenario launches the application and validates the required page/menu behavior.

The test uses:

* Selenium WebDriver
* Page Object Model
* TestNG
* ExtentReports

### Scenario 2

The second scenario launches the application and performs a product search.

**Test objective:**

> Search for **MacBook** as a product and verify the search result.

The scenario was successfully executed through the browser and the expected result was obtained.

## 🔄 Test Execution Flow

```text
TestNG Test
     ↓
BaseTest
     ↓
Open Browser
     ↓
Launch Application
     ↓
Page Object
     ↓
Perform Action
     ↓
Validate Result
     ↓
ExtentReport
     ↓
Close Browser
```

## 📊 Reporting

The framework uses **ExtentReports** to record test execution.

Reports are generated under:

```text
reports/
```

Screenshots generated during execution are stored under:

```text
screenshots/
```

TestNG execution results are available under:

```text
test-output/
```

## ▶️ How to Run

### Prerequisites

* Java JDK
* Maven
* Eclipse IDE (optional)
* Chrome browser or another supported browser

### Using Eclipse

1. Import the project into Eclipse as an existing Maven project.
2. Allow Maven to download the required dependencies.
3. Open:

```text
src/test/resources/testng.xml
```

4. Run the TestNG suite.
5. Review the generated reports and screenshots.

### Using Maven

From the project directory:

```bash
mvn test
```

## ⚙️ TestNG Suite

The TestNG suite is configured in:

```text
src/test/resources/testng.xml
```

The suite currently contains:

```text
MercariScenario01
MercariScenario02
```

## 🎯 What This Project Demonstrates

* Selenium WebDriver automation
* Java test automation
* Page Object Model
* PageFactory
* TestNG test execution
* Maven dependency management
* Browser-based testing
* Reusable page classes
* Test reporting with ExtentReports
* Screenshot capture
* Separation of test and page-object code

## 👨‍💻 Author

**Pradip Prasad**

Software Test Engineer | Automation | AI/GenAI Testing

📧 [pradippd31@gmail.com](mailto:pradippd31@gmail.com)
💼 [LinkedIn](https://www.linkedin.com/in/p31/)
💻 [GitHub](https://github.com/pradip-prasad)
