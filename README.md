# BeautyShop.pl — QA Testing Project

## About the Project

This project presents a QA testing process for the registration functionality of the BeautyShop.pl website.

The project was created as a portfolio example and includes both manual testing and, in the next stage, test automation.

The main goal was to verify whether the registration form works correctly for valid and invalid user input and to identify defects affecting the registration process.

## Testing Scope

The testing scope included:

* user registration with valid data
* email validation
* password validation
* password confirmation
* required field validation
* whitespace-only input
* Polish characters
* registration with an already registered email address
* terms and conditions acceptance

## Manual Testing

Manual testing was performed using:

* **Operating System:** Windows 11 Home
* **Browser:** Google Chrome

The manual testing documentation includes:

* test cases
* test execution results
* identified defects

### Test Cases and Execution Results

The complete set of test cases and their execution results is available here:

`manual-testing/test-cases-and-execution-result.pdf`

### Bug Reports

Identified defects are documented in separate bug reports:

* `manual-testing/bug-reports/bug-report-01.pdf`
* `manual-testing/bug-reports/bug-report-02.pdf`

## Defects Found

During testing, defects related to password validation and required fields were identified.

One of the documented issues concerns the validation of the password confirmation field. The field validates whether both password values are identical, but does not independently verify whether the main password meets the required validation rules.

The same behavior affects empty and whitespace-only input in the password confirmation field.

## Test Automation

The manual test cases will be automated using:

* **Playwright**
* **TypeScript**
* **Page Object Model (POM)**

The automated tests will cover the same registration scenarios tested manually.

The automation part of the project will be added to the repository in the `automation/` directory.

## Manual → Automation

The automated tests will correspond to the existing manual test cases:

| Manual Test Case | Automated Test           |
| ---------------- | ------------------------ |
| BSQA-T1          | Valid registration       |
| BSQA-T2          | Invalid email            |
| BSQA-T3          | Invalid password         |
| BSQA-T4          | Mismatched passwords     |
| BSQA-T5          | Polish characters        |
| BSQA-T6          | Required fields          |
| BSQA-T7          | Whitespace-only values   |
| BSQA-T8          | Already registered email |
| BSQA-T9          | Terms acceptance         |

## Technologies

### Manual Testing

* Test Case Design
* Functional Testing
* Negative Testing
* Boundary/Validation Testing
* Bug Reporting

### Test Automation

* Playwright
* TypeScript
* Page Object Model
* Test Fixtures
* Test Data Management
* HTML Test Reports
* GitHub Actions

## Project Structure

```text
beautyshop-manual-qa/
│
├── README.md
│
├── manual-testing/
│   ├── test-cases-and-execution-result.pdf
│   └── bug-reports/
│       ├── bug-report-01.pdf
│       └── bug-report-02.pdf
│
└── automation/
    ├── tests/
    ├── pages/
    ├── test-data/
    └── fixtures/
```

## Author

**Nikprzed**

QA Testing Portfolio Project
