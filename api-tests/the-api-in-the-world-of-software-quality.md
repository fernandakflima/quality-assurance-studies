# What is API?

Application Programming Interface

**Function:** Allow communication between applications/systems based on a service contract.

**What defines this contract?**

- The way in which the parties should communicate based on a request and its response.
- APIs must have good documentation so that they can be used correctly.

**Benefits:**

- Integration
- Innovation
- Expansion
- Maintenance

## Usage policies for APIs

- Public or open
- Private or internal
- From partners
- Composites

# Types (technologies) involving APIs

**REST - REpresentational State Transfer**

Architectural style with restrictions for creating applications under the HTTP protocol

**Uniform Interface**

- Required to decouple a client from the server
- Greater visibility
- Interface Controls:
     - Resource identification
     - Resource management by representations
     - Self-descriptive communications
     - Hypermedia as application state mechanism

**Client-Server**

- They work in isolation, with independent development

**Stateless**

- Calls can be made independently
- Each call must send data necessary to complete the request

**Use of layers**

- Greater scalability
- Greater security
- Greater performance of each module

**Code on demand**

- Possibility of services responding as a representation of a resource, information executable by the client
- reduces the number of resources to be implemented

**Cache usage**

- Data in a response can be cached

**Can return messages in different formats:**

- HTML
- XML
- text
-JSON

**SOAP - Simple Object Access Protocol**

- Simple object access protocol maintained by W3C and based on XML
- Created with the aim of enabling communication between different applications and platforms
- Supports communication protocols such as HTTP and SMTP

```
POST /InStock HTTP/1.1
Host: www.example.org
Content-Type: application/soap+xml; charset=utf-8
Content-Length: 299
SOAPAction: "http://www.w3.org/2003/05/soap-envelope"

<?xml version="1.0"?>
<soap:Envelope xmlns:soap="http://www.w3.org/2003/05/soap-envelope" xmlns:n="http://www.example.org">
    <soap:Header>
    </soap:Header>
    <soap:Body>
        <n:GetStockPrice>
            <n:StockName>T</m:StockName>
    </soap:Body>
</soap:Envelope>
```

**WebSocket API**

- Store status and data
- Communication is two-way, so either side can send a message to another party
- Single TCP connection
- Well used for IoT/Real-time applications

| Basis of comparison | WebSocket | REST |
|--------------------|-----------|------|
| **HTTP** | Usage on initial connection | Common in RESTful APIs |
| **Communication** | Bidirectional | Unidirectional |
| **Nature** | Socket-based | Resource-based |
| **Scenario** | Real-time applications | Too many GET requests |
| **Cost** | Bass | Bigger than WebSocket |
| **Performance** | High loads | Occasional communication |
| **State** | With status | Stateless |
| **Dependency** | IP and port only | HTTP methods |

**GraphQL**

- Query language for APIs, coming as an alternative to REST
- Not dependent on any specific bank
- Are organized in terms of types and fields, rather than endpoints
- Ease of maintenance

**RPC - Remote Procedure Calls**

- API is built based on the definition of methods that will be called via arguments

**Implementations:**

- XML-RPC
- JSON-RPC
- SOAP
- gRPC

# What does API testing consist of?

- Process of monitoring and validating requests and responses from an API, ensuring that it behaves as expected

**From the API we can evaluate:**
- Questions related to business rules before we reach the interface level
- Performance
- Integration with other APIs

## Approaches to API Testing

**Functional test:** We check if the API returns what is expected given a request

- Status code
- Schema

**Load test:** We check performance based on a large volume of requests in a short period

**Error detection:** We check if the API was well designed and if its errors are being well monitored and messages are clear

**Security:** We check how the API behaves and resists during attacks

**Penetration:** We check whether with little knowledge about the API we can attack an API

**Fuzz:** Sending random requests to analyze API behavior

## Importance of API testing

- We guarantee that the API behaves as it should in unexpected situations
- We guarantee that errors do not reach the level of interface testing
- We evaluate issues related to performance, performance and security earlier
- We check integration between APIs
- It is faster than Front-End tests

# Planning API tests

**What should I think about before starting the tests?**

- What life cycle model does the project follow?
- How many people are on the QA team?
- What is the prioritization of requirements?
- When is the deadline?
- What processes should we follow?
- What tools will my team and I use?

## Step 1: Review the API specification

Reviewing the API specification is important to understand the purpose, understand the relationship with business rules and understand what is expected from the request and response.

The way in which the specification will be created and maintained must be discussed by the team

- Standard for descriptions: OpenAPI
     - Definition of standards for describing language-independent HTTP-APIs

- Swagger: Tool that uses OpenAPI, and builds a range of utilities and facilities for generating, maintaining documentation and API testing

## Step 2: Determine the requirements and complexities

- What should be tested?
Status code, header, body...

- What is the complexity involved in coding the tests?
Infrastructure, Types of tests...

- What testing approaches?
- What integrations are there with the API?
- Which set of tests will be automated? And which ones will only be manuals?

- Which priority scenarios?
Success cases, error cases...

## Step 3: Determine the testing tool

- Postman/Insomnia
- SoapUI
- Katalon
- Assertible
- Tricentis Tosca
- API Fortress
- Mocklets
- Rest Assured
- Swagger
- Apache JMeter
- APIGee
- Cypress

Next note [here](https://github.com/fernandakflima/quality-assurance-studies/blob/main/api-tests/manual-and-automated-testing-with-postman.md)