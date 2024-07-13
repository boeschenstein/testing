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
- FakeLogger, TimeProvider <https://devblogs.microsoft.com/dotnet/fake-it-til-you-make-it-to-production/>
- <https://stackoverflow.com/questions/3459287/whats-the-difference-between-a-mock-stub>
  - `Dummy` objects are passed around but never actually used. Usually they are just used to fill parameter lists.
  - `Fake` objects actually have working implementations, but usually take some shortcut which makes them not suitable for production (an in memory database is a good example).
  - `Stubs`
    - provide canned answers to calls made during the test, usually not responding at all to anything outside what's programmed in for the test.
    - Stubs may also record information about calls, such as an email gateway stub that remembers the messages it 'sent', or maybe only how many messages it 'sent'.
  - `Mocks` are what we are talking about here: objects pre-programmed with expectations which form a specification of the calls they are expected to receive.
  - Snapshot testing
    - do not write asserts - use files instead
    - overview <https://timdeschryver.dev/bits/snapshot-testing-in-c-with-verify>
    - https://github.com/VerifyTests/Verify

## Advanced Testing

- More Information on DDD testing: https://github.com/boeschenstein/clean-architecture/blob/main/README.md
- SpecFlow (todo)

## Information

- Unit testing <https://docs.microsoft.com/en-us/dotnet/core/testing/>
- Integration Testing <https://docs.microsoft.com/en-us/aspnet/core/test/integration-tests>
- EF Core Testing: <https://docs.microsoft.com/en-us/ef/core/testing/>
