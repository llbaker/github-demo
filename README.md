# github-demo
A simple demo repository to show basic Git workflow


# Running Jest Unit Tests
Below is a compilation of commands for running jest unit tests from the command line using **jest version 27.4**.

## CLI format
Jest unit tests can be run using jest and nx.  Jest unit test can also be tun using yarn and npm. The format for each is

- `jest`*`option`*

- `nx test `*`option`*

- `yarn test`*`option`* 

- `npm test --`*`option`*


## Options for specifying which tests to run

| Action | jest | yarn | npm |
| :--- | :--- | :--- | :---- |
| Run all tests (default) | `jest`       | `yarn test`    | `npm test` |
| Run all tests in watch mode | `jest --watchAll`       | `yarn test --watchAll`    | `npm test -- --watchAll` |
| Run tests in watch mode with specified pattern, folder, etc | `jest --watch my-test`       | `yarn test --watch may test`    | `npm test -- --watch my-test` |
| Run only tests with specified pattern | `jest my-test` | `yarn test my-test` | `npm test -- my-test` |
| Run only tests in specified folder <br/>Windows: use `/` or `\\` <br/>as path separator `\` | `jest path/to/my-test` | `yarn path/to/my-test` | `npm test -- path/to/my-test` |
| Run only tests related to specified folders | `jest -- path/to/my-testA path/to/my-testB` | `yarn -- path/to/my-testA path/to/my-testB` | `npm test -- -- path/to/my-testA path/to/my-testB` |
| Run only tests on uncommitted files | `jest -o`       | `yarn test -o`    | `npm test -- -o` | 
| Run only tests with name in `describe`??? | `jest -t name-of-spec`       | `yarn test -t name-of-spec`    | `npm test -- -t name-of-spec` |
