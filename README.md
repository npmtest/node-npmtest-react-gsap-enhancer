# npmtest-react-gsap-enhancer

#### basic test coverage for  [react-gsap-enhancer (v0.3.0)](https://github.com/azazdeaz/react-gsap-enhancer)  [![npm package](https://img.shields.io/npm/v/npmtest-react-gsap-enhancer.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-react-gsap-enhancer) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-react-gsap-enhancer.svg)](https://travis-ci.org/npmtest/node-npmtest-react-gsap-enhancer)

#### Use the full power of React and GSAP together

[![NPM](https://nodei.co/npm/react-gsap-enhancer.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-gsap-enhancer)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-react-gsap-enhancer/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-gsap-enhancer/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-react-gsap-enhancer/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-react-gsap-enhancer/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-react-gsap-enhancer/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-react-gsap-enhancer/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-react-gsap-enhancer/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-react-gsap-enhancer/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-react-gsap-enhancer/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-gsap-enhancer/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-react-gsap-enhancer/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-react-gsap-enhancer/build/test-report.html](https://npmtest.github.io/node-npmtest-react-gsap-enhancer/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-react-gsap-enhancer/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-react-gsap-enhancer/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-react-gsap-enhancer/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-gsap-enhancer/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-gsap-enhancer/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-gsap-enhancer/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-react-gsap-enhancer/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-react-gsap-enhancer/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "react-gsap-enhancer",
    "version": "0.3.0",
    "description": "Use the full power of React and GSAP together",
    "main": "lib/index.js",
    "directories": {
        "example": "examples"
    },
    "scripts": {
        "start": "gulp",
        "coverage": "babel-node node_modules/.bin/isparta cover --report text --report lcov node_modules/.bin/_mocha -- --reporter dot",
        "lib": "rm -rf lib && babel ./src --out-dir lib  --source-maps --source-maps",
        "lib-watch": "npm run lib && babel ./src --out-dir lib  --source-maps --source-maps --watch",
        "browser-build": "webpack --config webpack.browser.config.js",
        "publish-browser": "npm run browser-build && gh-pages --dist browser --branch browser",
        "lint": "eslint --ignore-path .gitignore .",
        "test": "mocha --compilers js:babel-register",
        "test-debug": "node-debug _mocha --compilers js:babel/register"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/azazdeaz/react-gsap-enhancer.git"
    },
    "author": "Polgár András <azazdeaz@gmail.com>",
    "license": "MIT",
    "bugs": {
        "url": "https://github.com/azazdeaz/react-gsap-enhancer/issues"
    },
    "keywords": [
        "animation",
        "greensock",
        "gsap",
        "react",
        "react-component"
    ],
    "homepage": "https://github.com/azazdeaz/react-gsap-enhancer",
    "devDependencies": {
        "babel-cli": "^6.6.5",
        "babel-eslint": "^6.1.2",
        "babel-loader": "^6.2.4",
        "babel-plugin-dev-expression": "^0.2.1",
        "babel-preset-es2015": "^6.6.0",
        "babel-preset-react": "^6.5.0",
        "babel-preset-stage-1": "^6.5.0",
        "babel-register": "^6.7.2",
        "chai": "^3.2.0",
        "chai-spies": "^0.7.0",
        "component-playground": "^1.3.1",
        "coveralls": "^2.11.4",
        "custom-drag": "0.0.3",
        "eslint": "^3.3.0",
        "eslint-plugin-babel": "^3.3.0",
        "eslint-plugin-mocha": "^4.3.0",
        "eslint-plugin-react": "^6.1.0",
        "file-loader": "^0.8.4",
        "gh-pages": "^0.4.0",
        "gsap": "^1.18.0",
        "gulp": "^3.9.0",
        "gulp-gh-pages": "^0.5.2",
        "gulp-util": "^3.0.6",
        "history": "^1.13.1",
        "isparta": "^4.0.0",
        "lodash": "^3.10.1",
        "material-ui": "^0.15.4",
        "mocha": "^2.3.2",
        "node-libs-browser": "^0.5.2",
        "radium": "^0.18.1",
        "raw-loader": "^0.5.1",
        "react": "^15.3.2",
        "react-addons-transition-group": "^15.3.2",
        "react-dom": "^15.3.2",
        "react-motion": "^0.2.7",
        "react-router": "^1.0.0",
        "react-tap-event-plugin": "^1.0.0",
        "redux": "^0.12.0",
        "webpack": "^1.10.5",
        "webpack-dev-server": "^1.10.1"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
