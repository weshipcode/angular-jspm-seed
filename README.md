# angular-jspm-seed

AngularJS 1.x seed project using JSPM

## EditorConfig settings

The project is set up to use TABS for indentation by default.

Using tabs as opposed to spaces can eliminate uneven indentation.

See more details in the `.editorconfig` file.

## NPM scripts

### Linting Javascript

ESLint is used in this project to lint Javascript and warn for linting errors.

```
$ npm run lint
```

Every `.js` file under `app/` and `test/` folders will be linted.

### Running unit tests in browsers

Karma is used to run our unit test suites found under `test/` folder.

`$ npm run test`

Before running tests, `npm` will run the `lint` task on Javascript files, to make sure that there's no linting issues.
