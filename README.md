[![Build Status](https://travis-ci.org/pelevesque/is-offset.svg?branch=master)](https://travis-ci.org/pelevesque/is-offset)
[![Coverage Status](https://coveralls.io/repos/github/pelevesque/is-offset/badge.svg?branch=master)](https://coveralls.io/github/pelevesque/is-offset?branch=master)
[![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

# is-offset

Checks if a string is the offset of another.

## Node Repository

https://www.npmjs.com/package/@pelevesque/is-offset

## Installation

`npm install @pelevesque/is-offset`

## Tests

Command                      | Description
---------------------------- | ------------
`npm test` or `npm run test` | All Tests Below
`npm run cover`              | Standard Style
`npm run standard`           | Coverage
`npm run unit`               | Unit Tests

## Usage

### Parameters

```js
str1 (required)  
str2 (required)   
step (optional) default = 1
```

### Examples

```js
const isOffset = require('@pelevesque/is-offset')
```

```js
const str1 = 'abcd'
const str2 = 'efgh'
const result = isOffset(str1, str2)
// result === false
```

```js
const str1 = 'abcd'
const str2 = 'bcda'
const result = isOffset(str1, str2)
// result === true
```

```js
const str1 = '111222333444'
const str2 = '333444111222'
const step = 3
const result = isOffset(str1, str2, step)
// result === true
```
