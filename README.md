# Javascript library boilerplate

This is a basic boilerplate for small javascript libraries you want to write. It includes some essential gulp tasks which are already configured but you can change it of course.

## Usage

```bash
git clone git@github.com:nevyk/js-lib-boilerplate.git
mv js-lib-boilerplate <your-lib>
cd <your-lib>
npm install
npm init
```

Type some inital info of your library, start hacking and change the world. How easy!

## Gulp tasks

### gulp build

1. read files from src/
2. jshint
3. uglify
4. header
5. write files to dest/

### gulp test

1. read files from test/
2. test with mocha framework

_[expect.js](https://github.com/LearnBoost/expect.js) is used as default assertion library but you can install whatever you want_

## Licence

Tipograph is MIT licensed. Feel free to use it, contribute or spread the word. Created with love by Petr Nevyhoštěný ([Twitter](https://twitter.com/pnevyk)).