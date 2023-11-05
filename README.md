<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

[circleci-image]: https://img.shields.io/circleci/build/github/nestjs/nest/master?token=abc123def456
[circleci-url]: https://circleci.com/gh/nestjs/nest

  <p align="center">A progressive <a href="http://nodejs.org" target="_blank">Node.js</a> framework for building efficient and scalable server-side applications.</p>
    <p align="center">
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/v/@nestjs/core.svg" alt="NPM Version" /></a>
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/l/@nestjs/core.svg" alt="Package License" /></a>
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/dm/@nestjs/common.svg" alt="NPM Downloads" /></a>
<a href="https://circleci.com/gh/nestjs/nest" target="_blank"><img src="https://img.shields.io/circleci/build/github/nestjs/nest/master" alt="CircleCI" /></a>
<a href="https://coveralls.io/github/nestjs/nest?branch=master" target="_blank"><img src="https://coveralls.io/repos/github/nestjs/nest/badge.svg?branch=master#9" alt="Coverage" /></a>
<a href="https://discord.gg/G7Qnnhy" target="_blank"><img src="https://img.shields.io/badge/discord-online-brightgreen.svg" alt="Discord"/></a>
<a href="https://opencollective.com/nest#backer" target="_blank"><img src="https://opencollective.com/nest/backers/badge.svg" alt="Backers on Open Collective" /></a>
<a href="https://opencollective.com/nest#sponsor" target="_blank"><img src="https://opencollective.com/nest/sponsors/badge.svg" alt="Sponsors on Open Collective" /></a>
  <a href="https://paypal.me/kamilmysliwiec" target="_blank"><img src="https://img.shields.io/badge/Donate-PayPal-ff3f59.svg"/></a>
    <a href="https://opencollective.com/nest#sponsor"  target="_blank"><img src="https://img.shields.io/badge/Support%20us-Open%20Collective-41B883.svg" alt="Support us"></a>
  <a href="https://twitter.com/nestframework" target="_blank"><img src="https://img.shields.io/twitter/follow/nestframework.svg?style=social&label=Follow"></a>
</p>
  <!--[![Backers on Open Collective](https://opencollective.com/nest/backers/badge.svg)](https://opencollective.com/nest#backer)
  [![Sponsors on Open Collective](https://opencollective.com/nest/sponsors/badge.svg)](https://opencollective.com/nest#sponsor)-->

## Description

[Nest](https://github.com/nestjs/nest) framework TypeScript starter repository.

## Installation

```bash
$ npm install
```

## Running the app

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## Test

```bash
# unit tests
$ npm run test

# e2e tests
$ npm run test:e2e

# test coverage
$ npm run test:cov
```

## Support

Nest is an MIT-licensed open source project. It can grow thanks to the sponsors and support by the amazing backers. If you'd like to join them, please [read more here](https://docs.nestjs.com/support).

## Stay in touch

- Author - [Kamil Myśliwiec](https://kamilmysliwiec.com)
- Website - [https://nestjs.com](https://nestjs.com/)
- Twitter - [@nestframework](https://twitter.com/nestframework)

## License

Nest is [MIT licensed](LICENSE).


1. Initially, you were advised to install `@swc/cli` and `@swc/core` as development dependencies:

   ```bash
   npm i --save-dev @swc/cli @swc/core
   ```

2. You ran the following command:

   ```bash
   nest start -b swc
   ```

3. Your current project's package.json included the following dependencies:

   ```json
   "@nestjs/core": "^9.0.0",
   "@nestjs/common": "^9.0.0"
   ```

4. When running `nest start -b swc`, you encountered an error: "error: unknown option '-b'."

5. You decided to create a new project to see if the issue persisted:

   ```bash
   npx @nestjs/cli@9.0.0 new my-app-with-swc --skip-install
   ```

6. You noticed that a project created with NestJS version 10 required the following versions for `@nestjs/common` and `@nestjs/core`:

   ```json
   "@nestjs/common": "^10.0.0",
   "@nestjs/core": "^10.0.0"
   ```

7. You successfully ran the project with NestJS version 10 and found it to be faster in terms of build and start times.

8. You asked if it's necessary to use NestJS version 10. The answer is yes, as this feature is introduced in version 10.

8.1. You tried to create a project with NestJS version 9 to test this feature:

   ```bash
   npx @nestjs/cli@9.0.0 new my-app-with-swc --skip-install
   ```

9. You mentioned a feature to inform NestJS that `swc` should be used for building:

   ```bash
   nest start -b swc --type-check
   ```

   You also noted that you can add these settings to the `compilerOptions` in the `nest-cli.json` file.

10. You observed a decrease in test performance when using the `--type-check` flag. You asked whether additional configurations are needed for tests. Unit tests should be optimized.

11. You described the setup for SWC and Jest:

   - Installed the necessary packages:

     ```bash
     npm i --save-dev jest @swc/core @swc/jest
     ```

   - Updated the `transform` section in the `package.json` to use `@swc/jest` for transforming TypeScript/JavaScript files.

12. When running `npm run test:e2e`, you encountered the error "TypeError: _supertest is not a function."

13. To resolve this error, you changed the import statement from:

    ```javascript
    import * as request from 'supertest';
    ```

    to:

    ```javascript
    import request from 'supertest';
    ```

It appears that you've made several optimizations to your NestJS project, including the use of SWC and Jest, and resolved issues with imports. If you have any specific questions or need further assistance with any of the points mentioned, please feel free to ask.
