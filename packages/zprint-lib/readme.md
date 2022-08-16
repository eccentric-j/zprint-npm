# Zprint Library

Provides the [zprint](https://cljdoc.org/d/zprint/zprint/) API as a pre-compiled
js module to drop into node scripts.

## Installation

``` shell
npm install zprint-lib
```

## Usage

``` javascript
const zprint = require('zprint-lib')

zprint.formatFileStr("(ns my-project.core\n\t)", "my-project.core")
;; => "(ns my-project.core)"
```

## APIs

Check out https://cljdoc.org/d/zprint/zprint/1.2.4/doc/introduction for the
latest APIs but at the time of developing, this package provides the following APIs:

- configureAll
- czprint
- czprintStr
- setOptions
- zprint
- zprintFileStr
- zprintStr
