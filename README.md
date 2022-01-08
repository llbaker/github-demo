# github-demo
A simple demo repository to show basic Git workflow


# Running Jest Unit Tests
Below is a compilation of commands for running Jest unit tests from the command line using **jest version 27.4**.

## CLI format
Jest is the default test runner for applications and libraries created in Nx. The format for nx commands is

- `nx test [options]`
- `nx run <project>:test [options]`

## Options for specifying which tests to run
| Action |Nx|
| :--- | :---- |
| Run all tests (default) | `nx test`    |
| Run all tests in watch mode | `nx test --watchAll`    |
| Run tests in watch mode with specified pattern, folder, etc | `nx test --watch` |
| Run only tests on files affected by changes | `nx affected:test --watch` |
| Run only tests matching test-name string in describe<BR/>(enclose string in quotes when using phrase) | `nx test -t test-name`    |



| Run tests in watch mode with specified pattern, folder, etc | `nx test --watch=my-test` |
| Run only tests with specified pattern | `nx test my-test` |
| Run only tests in specified folder <br/>Windows: use `/` or `\\` <br/>as path separator `\` | `nx test path/to/my-test` |
| Run only tests related to specified folders | `nx test -- path/to/my-testA path/to/my-testB` |
| Run only tests on uncommitted files | `nx test -o` |



### Other options for specifying which test to run using jest, yarn, and npm
The formats for jest, yarn, and npm are

- `jest [option]`

- `yarn test [option]` 

- `npm test -- [option]`

These formats are provided for reference.

| Action | jest | yarn | npm |
| :--- | :--- | :--- | :---- |
| Run all tests (default) | `jest`       | `yarn test`    | `npm test` |
| Run all tests in watch mode | `jest --watchAll`       | `yarn test --watchAll`    | `npm test -- --watchAll` |
| Run tests in watch mode with specified pattern, folder, etc | `jest --watch my-test`       | `yarn test --watch my-test`    | `npm test -- --watch my-test` |
| Run only tests with specified pattern | `jest my-test` | `yarn test my-test` | `npm test -- my-test` |
| Run only tests in specified folder <br/>Windows: use `/` or `\\` <br/>as path separator `\` | `jest path/to/my-test` | `yarn path/to/my-test` | `npm test -- path/to/my-test` |
| Run only tests related to specified folders | `jest -- path/to/my-testA path/to/my-testB` | `yarn -- path/to/my-testA path/to/my-testB` | `npm test -- -- path/to/my-testA path/to/my-testB` |
| Run only tests on uncommitted files | `jest -o`       | `yarn test -o`    | `npm test -- -o` |
| Run only tests on files affected by changes | | | `npm run affected:test --watch` |
| Run only tests matching test-name string in describe<BR/>(enclose string in quotes when using phrase) | `jest -t test-name`       | `yarn test -t test-name`    | `npm test -- -t test-name` |


# Jest Unit Test - Starting Point #
Jest is the default test runner for Nx.

## Test Structure - Using Given-When-Then ##
By default, Jest uses a describe block that contains before-it-after structure for a set of tests. A single describe block can contain a describe block for each test case.
Shai Reznik’s jest-given plug-in, https://github.com/hirezio/given/tree/master/packages/jest-given, uses a given-when-then structure instead of the before-it-after structure.
### Installing Jest-Given ###

### Typical Test Structure ###
Unit tests are intended to test the methods of components.  

#### Testing Methods With Direct Inputs ####

#### Testing Methods With Indirect Inputs ####

#### Testing Methods With Collaboration Inputs ####



