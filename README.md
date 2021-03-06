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

```
$ npm run test
```

Before running tests, `npm` will run the `lint` task on Javascript files, to make sure that there's no linting issues.

### Linting SASS files

The Ruby tool `scss_lint` is being used to lint `.scss` files under `app/` folder.

```
$ npm run lint:sass
```

### Compiling SASS files

Via `node-sass`, the efficient `lib-sass` library is used to compile `.scss` files.

The main entry point is `app/main.scss` which will be loaded and compiled into plain CSS in `dist/main.css`.

```
$ npm run compile:sass
```

Before compiling `.scss` files, linting is being run against them. Any linting error will prevent the SCSS compilation.

### Watching files

#### Watching Javascript files

All `.js` files are being watched under `app/` and `test/` folders. On any file change the `test` task is run, including the linting beforehand.

```
$ npm run watch:js
```

#### Watching SASS files

All `.scss` files are being watched under `app/` folder. On any file change the `compile:sass` task is run, including the SCSS linting beforehand.

```
$ npm run watch:sass
```
