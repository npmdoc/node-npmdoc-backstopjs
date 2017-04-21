# npmdoc-backstopjs

#### api documentation for  backstopjs (v2.6.11)  [![npm package](https://img.shields.io/npm/v/npmdoc-backstopjs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-backstopjs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-backstopjs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-backstopjs)

#### BackstopJS: Catch CSS curveballs.

[![NPM](https://nodei.co/npm/backstopjs.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/backstopjs)

- [https://npmdoc.github.io/node-npmdoc-backstopjs/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-backstopjs/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-backstopjs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-backstopjs/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-backstopjs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-backstopjs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "backstopjs",
    "version": "2.6.11",
    "description": "BackstopJS: Catch CSS curveballs.",
    "bin": {
        "backstop": "./cli/index.js"
    },
    "scripts": {
        "lint": "npm run lint-web && npm run lint-node",
        "lint-web": "eslint --env browser compare/*.js compare/**/*.js --fix",
        "lint-node": "eslint --env node core/*.js core/**/*.js cli/*.js cli/**/*.js capture/*.js capture/**/*.js --fix",
        "genConfig": "node ./cli/index.js genConfig",
        "reference": "node ./cli/index.js reference",
        "test": "node ./cli/index.js test",
        "openReport": "node ./cli/index.js openReport",
        "echo": "node ./cli/index.js echo",
        "unit-test": "mocha --reporter spec --recursive test/",
        "integration-test": "rm -rf newdir && mkdir newdir && cd newdir && node ../cli/index.js genConfig && node ../cli/index.js reference && node ../cli/index.js test && node -e \"require('../')('test')\""
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/garris/backstopjs.git"
    },
    "author": "https://github.com/garris/BackstopJS/graphs/contributors",
    "license": "MIT",
    "main": "core/runner.js",
    "devDependencies": {
        "assert": "^1.4.1",
        "eslint": "^3.3.0",
        "eslint-config-semistandard": "^7.0.0-beta.0",
        "eslint-config-standard": "^6.0.0",
        "eslint-plugin-promise": "^3.3.0",
        "eslint-plugin-standard": "^2.0.0",
        "mocha": "^1.21.5",
        "mockery": "^1.4.0"
    },
    "dependencies": {
        "casperjs": "^1.1.0-beta5",
        "chalk": "^1.1.3",
        "fs-extra": "^0.30.0",
        "junitwriter": "~0.3.1",
        "minimist": "^1.2.0",
        "node-resemble-js": "^0.2.0",
        "object-hash": "1.1.5",
        "open": "0.0.5",
        "os": "^0.1.1",
        "p-map": "^1.1.1",
        "phantomjs-prebuilt": "^2.1.7",
        "temp": "^0.8.3"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
