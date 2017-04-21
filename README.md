# npmtest-spotify-web-api-node

#### basic test coverage for  [spotify-web-api-node (v2.3.6)](https://github.com/thelinmichael/spotify-web-api-node)  [![npm package](https://img.shields.io/npm/v/npmtest-spotify-web-api-node.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-spotify-web-api-node) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-spotify-web-api-node.svg)](https://travis-ci.org/npmtest/node-npmtest-spotify-web-api-node)

#### A Node.js wrapper for Spotify's Web API

[![NPM](https://nodei.co/npm/spotify-web-api-node.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/spotify-web-api-node)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-spotify-web-api-node/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-spotify-web-api-node/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-spotify-web-api-node/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-spotify-web-api-node/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-spotify-web-api-node/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-spotify-web-api-node/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-spotify-web-api-node/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-spotify-web-api-node/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-spotify-web-api-node/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-spotify-web-api-node/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-spotify-web-api-node/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-spotify-web-api-node/build/test-report.html](https://npmtest.github.io/node-npmtest-spotify-web-api-node/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-spotify-web-api-node/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-spotify-web-api-node/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-spotify-web-api-node/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-spotify-web-api-node/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-spotify-web-api-node/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-spotify-web-api-node/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-spotify-web-api-node/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-spotify-web-api-node/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "spotify-web-api-node",
    "version": "2.3.6",
    "homepage": "https://github.com/thelinmichael/spotify-web-api-node",
    "description": "A Node.js wrapper for Spotify's Web API",
    "main": "./src/server.js",
    "author": "Michael Thelin",
    "license": "MIT",
    "repository": {
        "type": "git",
        "url": "https://github.com/thelinmichael/spotify-web-api-node.git"
    },
    "dependencies": {
        "superagent": "^2.0.0"
    },
    "config": {
        "blanket": {
            "pattern": "src",
            "data-cover-never": "node_modules"
        }
    },
    "scripts": {
        "lint": "grunt jshint",
        "test": "npm run lint && ./node_modules/.bin/mocha --bail",
        "coveralls": "./node_modules/.bin/mocha -r blanket -R mocha-lcov-reporter | ./node_modules/coveralls/bin/coveralls.js"
    },
    "devDependencies": {
        "blanket": "^1.1.7",
        "coveralls": "^2.11.2",
        "grunt": "^1.0.1",
        "grunt-contrib-jshint": "~0.11.0",
        "grunt-contrib-watch": "~0.6",
        "grunt-simple-mocha": "0.4.x",
        "mocha": "~1.20.1",
        "mocha-lcov-reporter": "0.0.2",
        "mockery": "^1.4.0",
        "should": "~3.0",
        "sinon": "~1.12.2",
        "xunit-file": "0.0.5"
    },
    "keywords": [
        "spotify",
        "echonest",
        "music",
        "api",
        "wrapper",
        "client",
        "web api"
    ],
    "browser": {
        "./src/server.js": "./src/client.js"
    },
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
