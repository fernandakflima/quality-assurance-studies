# Test: Concepts and Objectives

## What is testing?

- Process of evaluating and reducing the risk of software failures in operation
- It is part of quality control
- The testing process is not just about the act of running a test

## General objectives

- Avoid defects and evaluate work products
- Check compliance with requirements
- Validate whether the product works as the customer expects
- Create confidence in the quality level of the tested object
- Risk reduction
- Work with the client to make decisions

## Testing VS Debugging

- Running tests may show failures caused by software defects.
- Debugging is already a process of investigating and correcting errors in the code development process
- These activities vary according to the methodology used in the team

## Testing principles

1. Testing shows the presence of defects and not their absence
2. Exhaustive testing is impossible
3. Initial testing saves time and money
4. Defects group together
5. The same test does not find new defects
6. Testing depends on context
7. The absence of errors is an illusion

# The testing process
## Influencing factors

- Lifecycle model
- Test levels and types
- Product and project risk
- Business domain
- Operational restrictions
- Organizational policies and practices
- Internal and external standards

## Testing activities

1. Test planning
2. Test monitoring and control
3. Test analysis
4. Test modeling
5. Test implementation
6. Test execution
7. Test completion

### Test planning

- Define test purposes
- Define the testing approach according to context constraints
- Specify tasks and deadline estimates

**Some strategies**

- Analytical: based on the analysis of some factor

- Model-based: designed based on a model of some necessary aspect of the product (business process model, state model, non-functional requirements model)

- Methodical: pre-defined set of tests, comparing important quality characteristics
- Process compatible: based on standards defined by the organization
- Directed: guided by stakeholders
- Regression: avoid regression of existing features
- Reactive: is reactive to the component or system and the events that occur during execution

### Test monitoring and control

- Continuous comparison of actual progress with the test plan based on output evaluation criteria... in other words, the 'done'!
- Use of progress reports

### Test analysis

- Test base is analyzed in order to analyze "what to test" according to pre-established criteria

    - Requirement specifications
    - Architecture documents, flowchart, use cases, etc...
    - Source code

- Evaluate the types of defects that can be found
- Define and prioritize test conditions

### Test modeling

- Answers the question "how to test?"
- Test conditions are elaborated into high-level test cases
- Prioritization of test cases and sets of test cases
- Verify necessary infrastructure and design test environment

### Test implementation

- Develop and prioritize automated testing procedures and possibly scripting
- Create test suites
- Logical and efficient organization of test execution
- Prepare test data

### Test execution

- Test suites are executed as planned, whether manually or automated
- Compare actual results with expected results
- Analyze anomalies to establish probable causes
- Report and record these anomalies
- Retest

### Test completion

- Collect data from testing activities already completed in order to review and consolidate experience
- Create test summary report
- Finalize and archive test data and records
- Improve maturity of the testing process

# Test levels
## What would these levels be?

These are groups of testing activities that are organized and managed together with respect to the level of development

- Component testing
- Integration testing
- System testing
- Acceptance test

### Component or unit testing

Focus on testing code components independently

**Important for:**

- Reduce risk
- Check functional and non-functional requirements
- Build component trust
- Find defects
- Prevent defects from being reflected in higher levels of testing

### Integration tests

Focus on integration between components or systems communication

**Important for:**

- Reduce risk
- Check interfaces
- Find defects in the parties involved that are reflected in higher levels of testing

### System testing

Focus on end-to-end system requirements

**Important for:**

- Reduce risk
- Validate system as a whole
- Find defects not seen at lower levels
- Prevent defects from being reflected in production after customer acceptance

### Acceptance tests

Focus on end-to-end system requirements from a validation and compliance standpoint with business rules and customer needs

**Important for:**

- Reduce risk
- Validate system as a whole
- Find defects not seen at lower levels
- Prevent defects from being reflected in production after customer acceptance

# Test types and objectives

Group of testing activities designed to verify specific characteristics of a system, based on specific objectives.

- Evaluate functional characteristics
- Evaluate non-functional characteristics
- Evaluate component/system structure or architecture
- Evaluate effects of changes in other parts of the code

## Functional test

- Assessment of functions that the system must perform
- Developed from requirements specifications, user stories, use cases
- Functional tests can be performed at all test levels
- Black box techniques are very useful for evaluating the system's functional behaviors

## Non-functional testing

- Assessment of non-functional characteristics such as usability, performance efficiency, security, etc…
- Can also be taken at all test levels

## White-box testing

- Focus on testing based on the internal structure of the system

    - Source code
    - Architecture
    - Data flow

- Code coverage with unit or integration tests

### Change testing

- Confirmation test: Verification after defect is corrected
- Regression testing: Checking side effects when changing a system component

# Objectives of the techniques

- Assistance in identifying test conditions, cases and their data

**Techniques:**

- Black box
- White box
- From experience

## Black box techniques

- Based on requirements documents, use cases, user stories, etc…
- Are applicable for functional or non-functional tests
- Focus on test inputs and outputs, abstracting the internal structure

1. Equivalence Partitioning
2. Limit value analysis
3. Decision table
4. State transition
5. Use case

### Equivalence partitioning

- Divides data into partitions or equivalence classes that are processed in the same way, in valid and invalid formats.

**Example:** An investment management and simulation system makes specific recommendations depending on age, having a risk score of 0-100:

- up to 18 years old: investments with risk 60-80
- 18 to 40 years old: investments with risk between 40-60
- age > 40: investments with lower risk
- the maximum age that the system makes predictions and simulations: 100 years

**Scenario to check investment simulation**

| Valid | Invalid |
|-------|---------|
| 0 - 18 | |
| 18 - 40 | |
| 40 - 100 | |
| | 100 > |

### Limit value analysis

- Extends equivalence partitioning when the partition is sorted and we can analyze the minimum and maximum value

**Example:** A merchandise shipping management system has the following rules:

- The customer does not pay shipping over 100 reais
- Between 50 and 100 reais, pay 20 reais
- Less than 50 reais, shipping goes up to 35 reais
- If the total purchase value reaches R$100,000, the customer must contact us directly or make a new purchase.

**Scenario to check shipping cost**

| Valid | Invalid |
|-------|---------|
| 0 - 50 | |
| 50 - 100 | |
| 100 - 100.000 | |
| | 0 < |
| | 100.000 > |

### Decision table

- Useful for testing requirements that specify conditions that combine with different results

| Variables | 1 | 2 | 3 | 4 |
|-----------|---|---|---|---|
| Valid card? | No | Yes | Yes | Yes |
| Valid password? | X | No | Yes | Yes |
| Amount requested is <= balance | X | X | No | Yes |
| Expected output | Invalid card | Invalid password | Insufficient balance | Withdrawal made successfully |

### State transition

Situations in which the system reacts differently to an event depending on current conditions or a history, which can be summarized as states

- A transition table is generated that will direct the test cases

| | Correct PIN | Incorrect PIN |
|-|-------------|--------------------------|
| S1) Start | S5 | S2 |
| S2) 1st attempt | S5 | S3 |
| S3) 2nd attempt | S5 | S4 |
| S4) 3rd attempt | S5 | S6 |
| S5) Access granted | - | - |
| S6) Account blocked | - |- |

### Use case testing

- Naturally derived from use cases
- Associate actions with the actors in the case
- Design tests for basic, alternative and error cases

## White-box techniques

- Based on the internal structure of the test object
- Can be used at all test levels
- Typically used for component-level testing in source code

1. Instruction Coverage
2. Decision coverage

### Instruction Coverage Test

- Tests executable code instructions
- Coverage measured as (number of instructions executed)/(total instructions)
- Tests the existing conditionals in the code and what is executed in each decision
- Coverage = number of decision results executed/ total decision results in the object
= 100% decision coverage –> 100% statement coverage

## Techniques based on experience

- Based on experience and intuition of those who test
- Situations not found in more systematic methods can be identified
- Coverage that is difficult to assess and measure

1. Error Assumption
2. Exploratory testing
3. Checklist-based