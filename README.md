# npmdoc-feed

#### api documentation for  [feed (v1.0.2)](http://projets.jpmonette.net/en/feed)  [![npm package](https://img.shields.io/npm/v/npmdoc-feed.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-feed) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-feed.svg)](https://travis-ci.org/npmdoc/node-npmdoc-feed)

#### Feed is a RSS and Atom feed generator for Node.js, making content syndication simple and intuitive!

[![NPM](https://nodei.co/npm/feed.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/feed)

- [https://npmdoc.github.io/node-npmdoc-feed/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-feed/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-feed/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-feed/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-feed/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-feed/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "feed",
    "version": "1.0.2",
    "description": "Feed is a RSS and Atom feed generator for Node.js, making content syndication simple and intuitive!",
    "homepage": "http://projets.jpmonette.net/en/feed",
    "author": "Jean-Philippe Monette <contact@jpmonette.net>",
    "contributors": [
        {
            "name": "Pierre Galvez"
        }
    ],
    "license": "MIT",
    "main": "lib/feed.js",
    "scripts": {
        "build": "rm -rf lib/ && mkdir lib && babel -d lib/ src/ --ignore **/*.spec.js -s",
        "prepublish": "npm run build",
        "test": "export NODE_ENV=test && jest",
        "test-travis": "export NODE_ENV=test && jest"
    },
    "jest": {
        "verbose": true,
        "collectCoverage": true,
        "collectCoverageFrom": [
            "**/src/*.{js}"
        ],
        "testMatch": [
            "**/*.spec.js"
        ]
    },
    "keywords": [
        "rss",
        "atom",
        "feed",
        "syndication",
        "xml",
        "wrapper",
        "blog"
    ],
    "dependencies": {
        "xml": ">= 0.0.5"
    },
    "devDependencies": {
        "babel-cli": "^6.24.0",
        "babel-preset-latest": "^6.24.0",
        "coveralls": "^2.13.0",
        "jest": "^19.0.2"
    },
    "engines": {
        "node": ">=0.4.0"
    },
    "bugs": {
        "url": "https://github.com/jpmonette/feed/issues"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/jpmonette/feed.git"
    },
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
