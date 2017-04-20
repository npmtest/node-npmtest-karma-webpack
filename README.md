# npmtest-karma-webpack

#### basic test coverage for  [karma-webpack (v2.0.3)](http://github.com/webpack/karma-webpack)  [![npm package](https://img.shields.io/npm/v/npmtest-karma-webpack.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-karma-webpack) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-karma-webpack.svg)](https://travis-ci.org/npmtest/node-npmtest-karma-webpack)

#### Use webpack with karma

[![NPM](https://nodei.co/npm/karma-webpack.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/karma-webpack)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-karma-webpack/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-karma-webpack/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-karma-webpack/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-karma-webpack/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-karma-webpack/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-karma-webpack/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-karma-webpack/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-karma-webpack/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-karma-webpack/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-karma-webpack/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-karma-webpack/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-karma-webpack/build/test-report.html](https://npmtest.github.io/node-npmtest-karma-webpack/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-karma-webpack/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-karma-webpack/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-karma-webpack/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-karma-webpack/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-karma-webpack/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-karma-webpack/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-karma-webpack/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-karma-webpack/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "karma-webpack",
    "version": "2.0.3",
    "author": "Tobias Koppers @sokra",
    "description": "Use webpack with karma",
    "license": "MIT",
    "homepage": "http://github.com/webpack/karma-webpack",
    "scripts": {
        "gulp": "gulp",
        "lint": "gulp lint",
        "clean": "gulp clean",
        "pretest": "npm run lint",
        "test": "npm run test.unit",
        "test.unit": "mocha --compilers js:babel-register --full-trace --check-leaks test/unit",
        "test.integration": "npm run build && karma start --single-run",
        "travis": "npm run test.unit && npm run test.integration",
        "travis:test": "npm run test.unit",
        "travis:lint": "npm run lint",
        "release": "standard-version",
        "release:tag:v2": "git push --follow-tags origin v2",
        "release:publish": "npm run build:release && npm publish --access public",
        "build:watch": "gulp build.watch",
        "build:release": "gulp",
        "build": "gulp build"
    },
    "files": [
        "lib",
        "index.js"
    ],
    "repository": {
        "type": "git",
        "url": "https://github.com/webpack/karma-webpack.git"
    },
    "peerDependencies": {
        "webpack": "^1.1.0 || ^2 || ^2.1.0-beta.0 || ^2.2.0-rc.0"
    },
    "dependencies": {
        "async": "~0.9.0",
        "loader-utils": "^0.2.5",
        "lodash": "^3.8.0",
        "source-map": "^0.1.41",
        "webpack-dev-middleware": "^1.0.11"
    },
    "devDependencies": {
        "babel-cli": "^6.11.4",
        "babel-core": "^6.11.4",
        "babel-plugin-transform-runtime": "^6.12.0",
        "babel-polyfill": "^6.9.1",
        "babel-preset-es2015": "^6.9.0",
        "babel-preset-stage-2": "^6.11.0",
        "babel-register": "^6.11.6",
        "chai": "^3.5.0",
        "chai-as-promised": "^5.3.0",
        "del": "^2.2.1",
        "eslint": "^3.1.1",
        "eslint-plugin-babel": "^3.3.0",
        "gulp": "github:gulpjs/gulp#4.0",
        "gulp-babel": "^6.1.2",
        "gulp-eslint": "^3.0.1",
        "gulp-util": "^3.0.7",
        "gulp-watch": "^4.3.9",
        "istanbul": "^0.4.4",
        "karma": "^1.x",
        "karma-chrome-launcher": "~1.0.1",
        "karma-mocha": "~1.1.1",
        "karma-spec-reporter": "~0.0.22",
        "mocha": "^2.5.3",
        "standard-version": "^4.0.0"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
