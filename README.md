# Cucumber Java Page Object Model Sample Framework

A starter framework for web automation using Java, Selenium, Cucumber, and Page Object Model.

## How to Download

- Clone:
  ```
  git clone https://github.com/prakashmanohara/cucumber-java-pom.git
  cd cucumber-java-pom
  ```
- Or download ZIP from the GitHub page.

## Setup

1. Install Maven: https://maven.apache.org/install.html
2. Install ChromeDriver and update the path in `DriverFactory.java`.
3. Run tests:
   ```
   mvn test
   ```

## Example Scenario

See [`features/login.feature`](features/login.feature):

```gherkin
Feature: Login

  Scenario: User logs in with valid credentials
    Given the user is on the login page
    When the user enters valid username and password
    And clicks the login button
    Then the user should be logged in successfully
```

## Page Object Example

See [`src/main/java/pages/LoginPage.java`](src/main/java/pages/LoginPage.java).
