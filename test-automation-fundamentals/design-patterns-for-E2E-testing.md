# Design patterns for testing

- Knowledge about design patterns is very important when we need to deal with highly complex projects.
- Test-oriented standards serve to solve common problems related to test consistency, cohesion, isolation, and accountability.

## POM - Page Object Model

**Pros:**

- Code reuse
- Cleaner code
- Ease of maintenance
- Independence of tests

**Cons:**

- Good understanding of programming and the pattern itself is required
- Elements are isolated to a specific page
- Good modeling is necessary, otherwise refactorings will be constant
- Complex projects require more time for automation

## App Actions

- The objective of App Actions is to use the Cypress architecture in favor of decoupling between the application layer and HTML
- Access to the application itself is used to configure the test status without depending on the UI, thus improving performance.

Next note [here](https://github.com/fernandakflima/quality-assurance-studies/blob/main/test-automation-fundamentals/material.md)