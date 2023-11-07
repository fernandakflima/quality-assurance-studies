# About Postman

Powerful Node.js-based *runtine* that allows you to add dynamic behavior to requests and *collections*

**Some important concepts:**

- *Collection:* Set of requests with the aim of keeping the space organized, collaborating with teams, generating documentation and running tests.
- *Pre-request script:* It is executed before a request is sent to the server.
- *Test script:* It is executed after sending the request and receiving the response.

**Some concepts about variables**
**Scope of variables:**

- Global - access across the entire workspace
- Ambient - different ambient settings
- From collection - specific to collection and independent of environment
- From external files - defined from CSV or JSON files
- Local - temporary variables created and accessed from individual scripts and override all other variables.

## Writing test scripts

- pm - javascript library object that provides functionality related to requests/responses
- It is possible to use the **require** command to import other libraries
- Tests can use the CHAI library syntaxr, using BDD
- Tests can use the concept of **expect**

Next note [here](https://github.com/fernandakflima/quality-assurance-studies/blob/main/api-tests/automated-testing-with-rest-assured.md)