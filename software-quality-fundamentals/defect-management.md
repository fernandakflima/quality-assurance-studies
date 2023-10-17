# Speaking of quality control
## Quality control

- Static analysis: evaluation of software documentation and source code
    - Code review
    - Code verification process automation tools
    - Analysis of stories and modeling

- Dynamic analysis: related to techniques with the running code
 Finally our beloved tests!

**Verification**: Ensure the product is being built correctly

**Validation** The correct product is being built

## Characterizing defects
### Defect tracking

- Understanding of the product and the types of defects found
- Facilitate correction of the process or product
- Report product status
- Alignment of reviews by the development team

### What is a defect?

- Generically means any type of anomaly found in the product

**Other definitions:**
- Error: Human action that produces an incorrect result
- Defect: Imperfection or deficiency related to product requirements and specifications
- System failure: Event in which the system does not perform a function under specific limits

### Reasons for errors

- Time pressure
- Human error
- Inexperience and/or lack of qualifications
- Lack of communication
- Code complexity, modeling, architecture…
- Technology complexity
- Unexpected ambient conditions

## Bug lifecycle: from tracking to reporting
### Life cycle

1. New: Defect is identified and registered for the first time
2. Assigned: defect is assigned for developer to evaluate
3. Open: developer starts analysis and correction
4. Fixed: Developer finalizes correction
5. Pending Retest: Waiting state for the test team
6. Retest: Retest execution status
7. Verified: Defect corrected
8. Reopen: Uncorrected defect.
9. Closed: Fixed + tested + approved
10. Duplicate: effect already found previously
11. Rejected: Defect is not new.
12. Deferred: Will be fixed in future versions.
13. Not a bug: When the anomaly is not in fact an error after analysis

### Important considerations

- The processes adapt to what your team and your product need!
- The team needs to agree and understand the entire defect tracking flow
- Defects can and should be tracked at any time in the software process life cycle.

**Main objectives of defect reports:**
- Provides interested parties with information regarding the anomalous event in order to attempt to isolate, reproduce and correct the problem or potential problem.
- Provides means to track product quality and their impact on testing and retesting activities
- Provides ideas for improving the development and testing process

- Good communication is essential!
- Efficient use of bug tracking and reporting tools
- Proactive team commitment in defect management

### Information from a defect report

- A unique identifier
- Title summarizing the problem
- Date/author
- Identification of the item under test and the environment
- Phase of the life cycle in which the defect was observed
- Full description of the defect for reproduction
- Evidence of assistance in resolution:
    - logs
    - database dumps
    - screenshots
    - recordings

- Expected outcome
- Severity
- Urgency
- Defect status
- Conclusions/Suggestions
- Impacts
- Historic
- Test reference