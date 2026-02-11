## About the Project

The goal of this project is to build an automated test suite for a publicly available demo webshop designed for testing purposes.
The tests are implemented using a Behavior-Driven Development (BDD) approach with Cucumber, based on predefined user stories.

The objective is to validate the webshop’s features through end-to-end automated tests that simulate real user interactions.
The project follows the Page Object Model (POM) design pattern to ensure maintainability, readability, and scalability of the test suite.


## Built With

* [![Java](https://img.shields.io/badge/Java-25-red?logo=openjdk&logoColor=white)](https://www.oracle.com/java/)
* [![Selenium](https://img.shields.io/badge/Selenium-WebDriver-43B02A?logo=selenium&logoColor=white)](https://www.selenium.dev/)
* [![Cucumber](https://img.shields.io/badge/Cucumber-BDD-23D96C?logo=cucumber&logoColor=white)](https://cucumber.io/)
* [![JUnit](https://img.shields.io/badge/JUnit-5-25A162?logo=junit5&logoColor=white)](https://junit.org/)
* [![Maven](https://img.shields.io/badge/Maven-Build-C71A36?logo=apachemaven&logoColor=white)](https://maven.apache.org/)
* [![IntelliJ IDEA](https://img.shields.io/badge/IntelliJ_IDEA-IDE-black?logo=intellijidea&logoColor=white)](https://www.jetbrains.com/idea/)
* [![Git](https://img.shields.io/badge/Git-latest-orange?logo=git&logoColor=white)](https://git-scm.com/)

## Prerequisites

* [![Java 25](https://img.shields.io/badge/Java-25-red?logo=openjdk&logoColor=white)](https://www.oracle.com/java/)
* [![Maven 3.9+](https://img.shields.io/badge/Maven-3.9-blue?logo=apachemaven&logoColor=white)](https://maven.apache.org/)
* [![Git](https://img.shields.io/badge/Git-latest-orange?logo=git&logoColor=white)](https://git-scm.com/)

## Getting Started

1. **Clone the repository** to your local machine:
```bash
git clone https://github.com/Daniel-Salyik/BetaShopAutomation.git
cd BetaShopAutomation
```

2. **Setup your environment**:
    - Create your own `env.local` file in `src/main/resources/Configuration/` based on the `env.example` file
    - Fill in the values as needed. You can find the required information on the demo webshop:
    - Set the `baseURL` to the demo webshop:
```
baseURL=https://www.saucedemo.com/
```

3. **Verify prerequisites**:
    - Ensure you have Java 25, Maven 3.9+, and Git installed

4. **Build the project**:
```bash
mvn clean compile
```

5. **Run the tests**:
```bash
mvn test
```
## Future Improvements

- **WebDriverManager integration** – simplify driver setup for different browsers
- **Setting up Selenium Grid with Docker support** – enable parallel and cross-browser test execution
- **Creating Cucumber reports** – generate detailed test reports for analysis and CI pipelines


### Project Structure

```
pom.xml
src
 ├── main
 │   ├── java
 │   │   └── com.BetaShop
 │   │       ├── pages
 │   │       └── utils
 │   └── resources
 │       └── configuration
 └── test
     ├── java
     │   └── com.BetaShopTests
     │       ├── hooks
     │       ├── stepdefinitions
     │       ├── pageTests
     │       └── utils
     └── resources
         └── features
```

