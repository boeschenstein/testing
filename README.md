# Testing

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
