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

Azure Pipelines see: https://github.com/boeschenstein/AzureDevOps/blob/main/README.md

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

## xUnit

<https://learn.microsoft.com/en-us/dotnet/core/testing/unit-testing-with-dotnet-test>

## Fake: Stub vs Mock

Speak the same Language: <https://learn.microsoft.com/en-us/dotnet/core/testing/unit-testing-best-practices#lets-speak-the-same-language>

## Best Practices

<https://learn.microsoft.com/en-us/dotnet/core/testing/unit-testing-best-practices>

## Unit Test Helpers

Examples: https://github.com/boeschenstein/aspnetefcore5-specification/blob/main/README.md#unit-test-helpers

- FluentAssertions
- Moq
- AutoMoqer/AutoMoqCore
- Bogus, AutoBogus
- AutoBogus / AutoFaker
- AutoFixture

## Unit Testing Tools

- FluentAssertions: <https://fluentassertions.com/>
- Moq, AutoMoq
  - <https://github.com/Moq>
  - <https://github.com/thomashfr/AutoMoqCore>
  - .NET classic, with example: <https://github.com/darrencauthon/AutoMoq>
- Bogus, AutoBogus, AutoFaker
    - <https://github.com/nickdodd79/AutoBogus>
    - Links and documentation: <https://github.com/bchavez/Bogus>
- Other libraries: 2 different `Faker.net`:
  - fakes data: addresses (UK, US), boolean, companies, countries, currencies, ...
  - A) <https://github.com/oriches/faker-cs> (based on ruby faker)
    - Nuget: <https://www.nuget.org/packages/Faker.Net>
  - B) <https://github.com/jonwingfield/Faker.Net> (based on ruby ffaker, sugar)
- AutoFixture: <https://github.com/AutoFixture/AutoFixture>
- Schouldly: <https://docs.shouldly.org/>
- Cheat Sheet Moq, xUnit, AutoFixture: <https://www.jankowskimichal.pl/wp-content/uploads/downloads/2016/01/Cheatsheet_Moq_xUnit_AutoFixture.pdf>

## Advanced Testing

- More Information on DDD testing: https://github.com/boeschenstein/clean-architecture/blob/main/README.md
- SpecFlow (todo)

## Information

- Unit testing <https://docs.microsoft.com/en-us/dotnet/core/testing/>
- Integration Testing <https://docs.microsoft.com/en-us/aspnet/core/test/integration-tests>
- EF Core Testing: <https://docs.microsoft.com/en-us/ef/core/testing/>
