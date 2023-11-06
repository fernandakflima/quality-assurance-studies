# Day in the life of a QA
## Writing user stories

### User stories

>As a customer, I want a screen to make payments via pix, as it is the easiest, fastest and freest way to make payments.

- Approach to structuring requirements from the user's perspective.

**Formula for capturing user stories:**

- Know who the user wants the functionality
- Know what the user wants
- Understand motivation and reason

- Use of other artifacts is welcome as long as they contribute to understanding: diagrams, flowcharts, mindmaps, prototypes, etc.
- Discussion with the team is essential for refinement

### Characteristics of a User Story

**INVEST**

- Independent
- Negotiable
- Valuable
- Estimable
- Small
- Testable

### Acceptance criteria

Confirmation that requirements have been met
- In the form of sentences like a checklist
- Use of Guerkin language (Given, Then, When)

### What should we pay attention to?

- Always analyze whether the story is focused on the user or customer
- User stories are different from well-defined and documented requirements
- Think about INVEST
- Think about quality requirements that are not thought of by the customer
- The User Story can and should be discussed by the team and created collaboratively
- Communication is essential

### An example of US

- Value delivery: objective of the functionality
- User narrative
- Technical requirements
     - Actors
     - Interfaces/Flows
     - Data
     - Business rules
     - Environment
     - Acceptance criteria

## Planning day

### Planning objectives

- Define and plan the items that will be developed in the sprint towards the product goal
- The entire scrum team participates

**Planning topics**

- Why will this sprint be valuable?
- What can be done?
- How will it be done?

### Understanding planning poker

**Objective:** Define estimates and size user stories and other valuable items for delivery.

**Problem:** We are terrible at estimating effort without a reference!

>Amount of effort involved in developing a feature + the complexity of this development + risk = story points

- It is important to use a reference measurement.
- Use of the Fibonacci sequence: avoids estimates without discussion and reflection, as scores drastically increase complexity.
- Hours can also be estimated according to the team's capacity, but it is not a measure directly proportional to story points.

>Effort is not complexity!

### The role of QA in planning

- Check whether User Stories are within a viable scope for delivery
- Verify that stories can be verified and validated within the correct period
- Analyze the complexity of the story with the devs without compromising quality
- QAs also participate in planning poker

### Planning and estimating QA activities

- Testability is part of the complexity of the story.
- Manual testing is time-consuming and involves experience and knowledge, therefore, it is better to overestimate than underestimate the activities.
- Dividing tasks objectively helps in dividing hours

     - Survey and writing of scenarios, test cases and/or mindmaps
     - Execution of manual tests
     - Automated tests

## Test documentation: mindmap, test cases and scenarios

### Planning defined, now what?

- Test planning is constantly adapted during the sprint, however it is a fact that before executing any test it is necessary to think about:

     - Technique to be used
     - Type and Level of the test
     - Data

### Documentation in the agile world

>Documents are meant to be read!

- Relying on memory is always not an option!
- It must be the minimum necessary for there to be tracking of validated scenarios and cases
- It is important to reevaluate and add new tests
- Important for the team's collaborative attitude
- Important for customer follow-up
- Use test management tools to simplify creation
     - **Test plan:** Involves the set of strategies and test cases for a specific functionality or set of functionalities.
     - **Test cycle:** Involves the set of test cases to be executed in accordance with what is established in a test plan.
     -**Test Cases/Scenarios:** Documents that define what to test or how a functionality should be tested,

### Scenarios VS Test Cases

- **Test cases:** Set of actions to verify a functionality in a more specific way.
     - Steps
     - Data
     - Preconditions
     - Postconditions

- **Test scenario:** A functionality situation that can be tested from a higher level view
     - Derives test cases

### Using MindMaps

Visual tool to "construct thought"!

Suitable for any context where a lot of information is needed and linked to a topic.

It may be useful for:

- Test plan
- Test scenarios
- Any context that requires the construction of ideas!