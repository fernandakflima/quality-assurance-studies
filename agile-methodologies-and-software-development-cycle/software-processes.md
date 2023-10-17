# Defining Process, Flow and Software Standards

>"... Software development is a social learning process. It is an iterative process in which the evolving tool itself serves as a means of communication
..." - Howard Jr. quote (apud Pressman, Roger S., Maxim, Bruce R. Engenharia de Software: Uma Abordagem Profissional, 8°ed)

## What is Software Process?

Methodology for the activities, actions and tasks necessary to develop software.

It's like a script.

### Main process activities

- Communication
- Planning
- Modeling
- Construction
- Delivery

### Process Flow

- Flow process linear
- Flow process interactive
- Flow process evolutionary
- Flow process parallel

### Process Standards

- Describes a process problem and suggests solutions according to the context
- Can be set to any level of abstraction

## Prescriptive Model

- Also called "traditional" models
- Focus on the order and consistency of the process
- Prescribe a set of process elements and flows

### Waterfall Model - Classic

- Useful for well-understood, defined and stable requirements
- Linear and systematic process

#### Negative points of the Waterfall Model

- Real projects do not follow sequential flows
- Does not deal well with constant adaptation to change
- Requirements are not well established in the first phase
- Long time to view the first version of the software
- Generates blocking states for the team

### Model V

- Relationship between quality assurance activities and remaining process activities
- There is no fundamental difference between Waterfall and V

## Incremental, Evolutionary and Concurrent Models
### Incremental Process Models

- Situations with well-defined but unrefined initial requirements
- Models: prototyping

### Evolutionary Process Model

- Model that enables the development of software that constantly grows and adapts
- They are iterative
- Models: prototyping and spiral

### Evolutionary Process Model - Prototyping

- Useful for refining requirements
- Validate efficiency and user interaction
- Can be applied alone or in conjunction with other processes
- The prototype acts as a way of obtaining requirements
- Can be disposable or can evolve

#### Negative points of prototyping

- Does not consider the overall quality of software after prototyping is considered "functional"
- Accommodate with initial prototyping choices

### Evolutionary Process Model - Spiral

- Iterative nature of prototyping, plus the systematic aspects of waterfall
- Incremental cyclical strategy focused on reducing risks

### Concurrent Process Model

- Concurrent representation of activities of any process

## Specialized Models
### Component-based

- Development based on components with defined interfaces to be integrated into the software
- Evolutionary in nature
- Focus on reuse

### Formal Method Models

- Activities based on leading to the formal mathematical specification of the software
- Mathematical analysis assists in discovering ambiguities or inconsistencies
- Development consumes time and money
- Complexity requires education and training
- Well regarded for software with critical factors

### Aspect-oriented Models

- Paradigm that offers a methodological and process approach to define, specify, design and build aspects, which are points of interest that propagate and intersect other parts of the application

## Unified Process
### Phases of the Unified Process

1. Design phase

    Communication and planning
    - Requirements are described in sets of preliminary use cases
    - Identification of resources, risks, schedule, etc.

2. Elaboration phase

    Planning and modeling
    - Refinement and expansion of use cases
    - Expansion of architectural representation

3. Construction phase
    - Software development based on models
    - Use of models to generate acceptance test suite
    - Use of tests according to development

4. Transition phase

    Construction and delivery
    - Common delivery with beta tests to receive feedback
    - The increment becomes a usable version of the software

5. Production phase

    Delivery
    - Continuous usage monitoring
    - Support
    - Reports for defects and changes