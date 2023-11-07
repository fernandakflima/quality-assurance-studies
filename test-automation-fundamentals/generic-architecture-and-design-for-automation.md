# Generic automation architecture

- Concepts about software architecture
- Generic architecture for automation projects
- What to consider before starting a project
- Approaches to test case automation

## What is software architecture?

- Description and understanding of the system components, their structures and relationships.
- Consider external factors when defining a system’s architecture.

## Thinking about architectural patterns

- They are general and reusable solutions to solve recurring problems within a certain context
- Are inserted in a larger scope of the system

## Design patterns

They are general, reusable solutions to common problems related to language-independent software project construction

**They are divided into:**

- Creation patterns: factory method, abstract factory, singleton...
- Structural patterns: adapter, composite, facade, proxy...
- Behavioral patterns: command, observer, mediator...

## SOLID

- **Single responsibility:** Each component must have a single responsibility and this must be encapsulated.
- **Extension:** Each component must be open for extension, but closed for modification.
- **Replacement:** Each component must be replaceable without affecting the overall behavior of the solution.
- **Segregation:** It is better to have specific components than a general multipurpose component.
- **Dependency inversion:** Components must depend on abstractions and not on lower-level details.

# Automation project architecture

## Test generation layer

- Manual creation of test cases
- Developing, capturing or obtaining test data
- Automatic generation of test cases from models

## Test definition layer

- Specification of test cases
- Definition of test data
- Specification of testing procedure
- Definition of scripts to execute test cases
- Grant access to test libraries as needed

## Test execution layer

- Automatically run test cases
- Register executions
- Report executions

## Test adaptation layer

- Control test environment
- Interact with the system to be tested
- Monitor the system being tested
- Simulate or emulate the environment being tested

## Automated testing solution project management

- Pay attention to project configuration management
- Versioning must follow good practices
- Extraction of metrics should be analyzed in the same way as in a manual approach

# What should we consider before starting a project?

- Which activity or phase of the testing process do we want to automate?
- What level of testing do we want to support?
- What type of test is it?
- Who will run and implement the test?
- Which projects are free and which can be purchased?
- What technologies do we want to support? And the complexity?
- What languages do we want to use?
- Which software life cycle model are we included in?
- How complex is implementation and how does it affect the project?
- Will training be necessary?

# Approaches to automation

We know that test cases correspond to the sequence of actions performed on the system being tested.

- The solution implements test cases directly into automated test scripts
- The solution designs test procedures and turns them into automated scripts
- The solution uses a tool to translate test procedures into automated test scripts
- The solution uses a tool that generates automated test procedures or translates scripts directly from models

## Capture and playback approach

The tools are used to capture the interaction with the system while executing the sequence of actions, recording the outputs. Output checking can be manual or automated.

**Pros:** Easy to use and configure
**Cons:** Difficult to evolve and maintain

## Generation of Linear Scripts

The tools are used to capture the interaction with the system while executing the sequence of actions, recording the outputs and generating linear test scripts.

**Pros:** Easy to use and configure
**Cons:** Difficult to evolve and maintain

## Generation of Structured Scripts

Generation of reusable script libraries for test cases.

**Pros:** Lower maintenance and lower cost for new tests
**Cons:** Higher cost for creating shared scripts. Good programming skills required

## Data-driven

Approach in which scripts use files with different masses of data.

**Pros:** Reduces the cost of adding tests. Increase variations with test data.
**Cons:** Manage the files to be read by the solution well

## Use of keywords

The keyword-based script uses definition files based on more descriptive words in addition to the possibility of using data files

**Pros:** Reduces the cost of adding tests. Increase variations with test data
**Cons:** Implementing keywords comes with a cost. Good keywords are more reused

## Model-based testing

Automated test case generation as opposed to test case execution. You can derive any type of script.

**Pros:** Abstraction ensures focus on the test objective. Maintenance only on models.
**Cons:** Good knowledge is required for testing models in addition to ensuring that the generation tools are mature and generate good reports.

## Behavior-Driven Testing (BDD)

Use of natural language to define the behavior of the functionality.

**Pros:** Greater business understanding. Ease of creating case modeling.
**Cons:** Ambiguity. It can generate repeated code if not well thought out.
​
Next note [here](https://github.com/fernandakflima/quality-assurance-studies/blob/main/test-automation-fundamentals/design-patterns-for-E2E-testing.md)