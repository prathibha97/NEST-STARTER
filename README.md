## Description

[NestJS Scaffold Project](https://github.com/OctaCode-BL/nestjs-scaffold-project.git) that we from [OctaCode](https://octacode.ba) use to spin up our projects.

## Prerequisites

You will need [pnpm](https://pnpm.io/installation) for running this repository.

## Installation

```bash
$ pnpm install
```

## Running the app

```bash
# development
$ pnpm run start

# watch mode
$ pnpm run start:dev

# production mode
$ pnpm run start:prod
```

## Test

```bash
# unit tests
$ pnpm run test

# e2e tests
$ pnpm run test:e2e

# test coverage
$ pnpm run test:cov
```

## Linting

```bash
# linting file and folder names
$ pnpm run ls-lint

# linting project code
$ pnpm run lint

# Linting both as in the pre-commit hook
$ pnpm run pre-commit
```

## Pre-Commit Hook

We use pre-commit hook to lint and test our code before committing it and eventually landing it on the repository. This way we keep our code clean and concise.

In order to get it working, please execute following commands:

```bash 
$ npm pkg set scripts.prepare="husky install"
$ npm run prepare
```

This edits package.json and prepares script for husky. You only need to run it once.

Then you can add a hook:

```bash
$ npx husky add .husky/pre-commit "pnpm run pre-commit"
$ git add .husky/pre-commit
```


## Recommended VS Code extensions

This repository also includes recommended extensions that we use with VS Code. If you don't use VS Code, you can just remove the folder .vscode.

Happy hacking!
OctaCode Team
