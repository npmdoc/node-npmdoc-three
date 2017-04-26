# npmdoc-three

#### basic api documentation for  [three (v0.85.2)](http://threejs.org/)  [![npm package](https://img.shields.io/npm/v/npmdoc-three.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-three) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-three.svg)](https://travis-ci.org/npmdoc/node-npmdoc-three)

#### JavaScript 3D library

[![NPM](https://nodei.co/npm/three.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/three)

- [https://npmdoc.github.io/node-npmdoc-three/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-three/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-three/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-three/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-three/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-three/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "mrdoob"
    },
    "bugs": {
        "url": "https://github.com/mrdoob/three.js/issues"
    },
    "dependencies": {},
    "description": "JavaScript 3D library",
    "devDependencies": {
        "electron": "^1.6.1",
        "eslint": "^3.10.1",
        "eslint-config-mdcs": "^4.2.2",
        "qunitjs": "^2.1.1",
        "rollup": "^0.41.4",
        "rollup-watch": "^3.2.2",
        "uglify-js": "^2.6.0"
    },
    "directories": {
        "doc": "docs",
        "example": "examples",
        "test": "test"
    },
    "dist": {
        "shasum": "8936f89c3668f7bf12f9b085ddf5dd409916ea27",
        "tarball": "https://registry.npmjs.org/three/-/three-0.85.2.tgz"
    },
    "eslintConfig": {
        "extends": "mdcs"
    },
    "files": [
        "package.json",
        "bower.json",
        "LICENSE",
        "README.md",
        "build/three.js",
        "build/three.min.js",
        "build/three.module.js",
        "src",
        "examples/js",
        "examples/fonts"
    ],
    "gitHead": "a1fb0b5b3ffd766f7d58cc4ec065c6b9bd617e81",
    "homepage": "http://threejs.org/",
    "jsnext:main": "build/three.module.js",
    "keywords": [
        "three",
        "three.js",
        "3d",
        "webgl"
    ],
    "license": "MIT",
    "main": "build/three.js",
    "maintainers": [
        {
            "name": "bhouston"
        },
        {
            "name": "cabbibo"
        },
        {
            "name": "mrdoob"
        }
    ],
    "module": "build/three.module.js",
    "name": "three",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mrdoob/three.js.git"
    },
    "scripts": {
        "build": "rollup -c",
        "build-closure": "rollup -c && java -jar utils/build/compiler/closure-compiler-v20160713.jar --warning_level=VERBOSE --jscomp_off=globalThis --jscomp_off=checkTypes --externs utils/build/externs.js --language_in=ECMASCRIPT5_STRICT --js build/three.js --js_output_file build/three.min.js",
        "build-test": "rollup -c test/rollup.unit.config.js",
        "build-uglify": "rollup -c && uglifyjs build/three.js -cm --preamble \"// threejs.org/license\" > build/three.min.js",
        "dev": "rollup -c -w -m inline",
        "editor": "electron ./editor/main.js",
        "lint": "eslint src",
        "test": "rollup -c test/rollup.unit.config.js -w"
    },
    "version": "0.85.2",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
