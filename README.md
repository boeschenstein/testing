# Testing

## Continuous Delivery (CD) Pipeline

From 'Continuous delivery and continuous deployment': <https://youtu.be/bTGj4PeRPjs>

1. Source Control Management
1. CI - Continuous Integration
    - Integration tests
    - Unit tests
1. System Integration Tests (SIT)
1. Operational Acceptance Tests (OAT)
1. Security Tests (Pen)
1. Compliance Tests
1. Deploy
1. Delivery

## Seven Software Testing Principles

From: <https://www.guru99.com/software-testing-seven-principles.html>

- Principle 1 Testing shows presence of defects
- Principle 2 Exhaustive testing is impossible
- Principle 3 Early Testing
- Principle 4 Defect Clustering
- Principle 5 Pesticide Paradox
- Principle 6 Testing is context dependent
- Principle 7 Absence of errors - fallacy

## Continuous Integration (CI)

<https://youtu.be/RcTFpNlkiUs>

## Unit Testing

![image](https://user-images.githubusercontent.com/38001274/200137405-897b22b6-d97e-45ed-a0d0-ed116d161e13.png)

## TDD - Test driven Developmenet

what        | why         | how
----------- | ----------- | --------------
unit        | functional  | autmated
integration | acceptance  | semi-automated
component   | smoke       | manual
service     | exploratory | 
UI          |             | 

Book: Succeeding with agile

| costs | Type          | number of tests  | 
| :---: | :-----------: | :--------------: | 
| ++++  | Manual tests  | +                | 
| +++   | UI tests      | ++               | 
| ++    | Service tests | +++              | 
| +     | Unit tests    | ++++             | 

### Acceptance Tests

- Verify functionality
- Language of business
- Criteria of completeness
- Full tests are problematic

How

- Eliminate UI
- Use In-Memory DB 
- Mock Infrastructure 
- Mock Cross-Cutting concernes

What

- Focus on essential
- Minimize coded UI-Test
- Smoke tests instead
- Minimize manual tests
- Exploratory tests instead
