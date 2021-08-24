## About

This will make you understand how to implement your e2e tests using Cypress and do continuous integration and delivery with CircleCI for your tests.

## Table of Contents

- [INIT Project](#Init-Project)
- [Setup your CircleCI account](#Setup-your-CircleCI-account)

# Init-Project

1. Clone the project locally, Run command:

```
git clone https://github.com/Dikshita25/circleCI-cypress.git
```

2. Go to the project root directory, Where the project is cloned in the system:

```
cd circleCI-cypress
```

3. Run all e2e Tests via command:

```
npm run cypress run --browser chrome
```

The output of the result would something like:

       Spec                                              Tests  Passing  Failing  Pending  Skipped

┌────────────────────────────────────────────────────────────────────────────────────────────────┐
│ ✔ tests/verifySite.js 00:08 3 3 - - - │
└────────────────────────────────────────────────────────────────────────────────────────────────┘
✔ All specs passed! 00:08 3 3 - - -

# Setup-your-CircleCI-account

1.  You can login to CircleCI portal via gitHub and you'll have access to all your github repositories within the Project listing screen.

2.  Inorder to setup circleci for your github project, select Setup project. This will then ask you to choose the branch from which you want to execute your tests and it should contain the config.yml inside .circleci folder. Or another option would be to create a new config file.

**Note**: For this project, we are triggering the pipeline manually. But you can definitely, automate the pipeline trigger process.

3.  As you setup the project, the pipeline would be triggered automatically and the build progress can be seen
