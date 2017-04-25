# npmtest-electron-rebuild

#### basic test coverage for  [electron-rebuild (v1.5.7)](https://github.com/electron/electron-rebuild)  [![npm package](https://img.shields.io/npm/v/npmtest-electron-rebuild.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-electron-rebuild) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-electron-rebuild.svg)](https://travis-ci.org/npmtest/node-npmtest-electron-rebuild)

#### Electron supporting package to rebuild native node modules against the currently installed electron

[![NPM](https://nodei.co/npm/electron-rebuild.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/electron-rebuild)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-electron-rebuild/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-electron-rebuild/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-electron-rebuild/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-electron-rebuild/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-electron-rebuild/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-electron-rebuild/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-electron-rebuild/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-electron-rebuild/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-electron-rebuild/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-electron-rebuild/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-electron-rebuild/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-electron-rebuild/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-electron-rebuild/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-electron-rebuild/build/test-report.html](https://npmtest.github.io/node-npmtest-electron-rebuild/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-electron-rebuild/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-electron-rebuild/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-electron-rebuild/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-electron-rebuild/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-electron-rebuild/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-electron-rebuild/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-electron-rebuild/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-electron-rebuild/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Paul Betts"
    },
    "babel": {
        "presets": [
            "es2015"
        ],
        "plugins": [
            "transform-runtime",
            "syntax-async-functions",
            [
                "transform-async-to-module-method",
                {
                    "module": "bluebird",
                    "method": "coroutine"
                }
            ]
        ]
    },
    "bin": {
        "electron-rebuild": "lib/cli.js"
    },
    "bugs": {
        "url": "https://github.com/electron/electron-rebuild/issues"
    },
    "dependencies": {
        "babel-register": "^6.16.3",
        "babel-runtime": "6.18.0",
        "bluebird": "^3.4.6",
        "colors": "^1.1.2",
        "debug": "^2.4.5",
        "fs-promise": "^1.0.0",
        "node-abi": "^1.0.3",
        "node-gyp": "^3.4.0",
        "ora": "^0.3.0",
        "rimraf": "^2.5.0",
        "spawn-rx": "^2.0.7",
        "yargs": "^3.31.0"
    },
    "description": "Electron supporting package to rebuild native node modules against the currently installed electron",
    "devDependencies": {
        "babel-cli": "^6.5.2",
        "babel-plugin-syntax-async-functions": "^6.13.0",
        "babel-plugin-transform-async-to-module-method": "^6.16.0",
        "babel-plugin-transform-runtime": "^6.15.0",
        "babel-preset-es2015": "^6.16.0",
        "chai": "^3.4.1",
        "chai-as-promised": "^6.0.0",
        "electron-prebuilt": "^1.4.12",
        "mocha": "^3.2.0"
    },
    "directories": {},
    "dist": {
        "shasum": "bb681850456de5c8d5405cbc1b4ae3d0752f1b52",
        "tarball": "https://registry.npmjs.org/electron-rebuild/-/electron-rebuild-1.5.7.tgz"
    },
    "engines": {
        "node": ">=6.0.0"
    },
    "gitHead": "8288c332f2708915d29aa49be229a6f8a24ab426",
    "homepage": "https://github.com/electron/electron-rebuild",
    "keywords": [
        "electron"
    ],
    "license": "MIT",
    "main": "lib/main.js",
    "maintainers": [
        {
            "name": "electron"
        },
        {
            "name": "jlord"
        },
        {
            "name": "kevinsawicki"
        },
        {
            "name": "paulcbetts"
        },
        {
            "name": "zcbenz"
        },
        {
            "name": "zeke"
        }
    ],
    "name": "electron-rebuild",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/electron/electron-rebuild.git"
    },
    "scripts": {
        "compile": "babel -d lib/ src/ && babel -d test-dist/ test/",
        "prepublish": "npm run compile",
        "test": "npm run compile && mocha test-dist/* --timeout 120000"
    },
    "version": "1.5.7"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
