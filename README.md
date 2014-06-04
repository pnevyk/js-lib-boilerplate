# Javascript library boilerplate

This is a basic boilerplate for small javascript libraries you want to write. It includes some essential gulp tasks which are already configured but you can change it of course.

## Usage

```sh
git clone git@github.com:nevyk/js-lib-boilerplate.git # clone repo
mv js-lib-boilerplate <your-lib>                      # rename folder
cd <your-lib>                                         # got to the folder
rm -rf .git                                           # delete .git folder
git init                                              # initialize empty repo
npm init                                              # initialize npm package
npm install                                           # install dependencies
```

Type some inital info of your library, start hacking and change the world. How easy!

## Gulp tasks

### gulp

1. `gulp clean`
2. `gulp build`
3. `gulp test`
4. `gulp lint`

### gulp build

1. read files from `src/`
2. concat files to one file
3. wrap the whole code with immediately-invoked function expression
4. beautify the code
5. write the file to `dest`
6. minify the code with uglify
7. add header to minified file
8. rename the file to have `.min` suffix
9. write the file to `dest/`

### gulp clean

1. read files from `dest/`
2. delete them with clean

### gulp lint

1. read files from `src/`
2. concat files to one file
3. wrap the whole code with immediately-invoked function expression
4. lint files with jshint
5. display jshint errors with default reporter

### gulp test

1. read files from `test/`
2. test with mocha framework

_[expect.js](https://github.com/LearnBoost/expect.js) is used as default assertion library but you can install whatever you want_

### gulp watch

1. watches changes in `src/`
2. runs default task when change occurs

### gulp watch:build

1. watches changes in `src/`
2. runs `gulp clean` and `gulp build` when change occurs

### gulp watch:test

1. watches changes in `src/` and `test/`
2. runs `gulp test` when change occurs

## Licence

Tipograph is MIT licensed. Feel free to use it, contribute or spread the word. Created with love by Petr Nevyhoštěný ([Twitter](https://twitter.com/pnevyk)).