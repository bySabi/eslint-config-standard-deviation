# eslint-config-standard-deviation

[![npm version](https://badge.fury.io/js/eslint-config-standard-deviation.svg)](https://badge.fury.io/js/eslint-config-standard-deviation)
[![npm downloads](https://img.shields.io/npm/dm/eslint-config-standard-deviation.svg?style=flat-square)](https://www.npmjs.com/package/eslint-config-standard-deviation)
[![Known Vulnerabilities](https://snyk.io/test/github/bysabi/eslint-config-standard-deviation/badge.svg)](https://snyk.io/test/github/bysabi/eslint-config-standard-deviation)

> ESLint [shared configuration](http://eslint.org/docs/developer-guide/shareable-configs) for javascript `ES5`, `ES2015`, `ES.next` and `React` projects based on `standard` shared eslint-config


* [eslint-config-standard][standard]
* [eslint-config-standard-react](https://github.com/feross/eslint-config-standard-react)


## What is different from `standard` eslint-config ?
[standard][standard] shared eslint-config rules are almost fine but we do not like to force us to ...
* not use semicolon `;`
* put space before function parens `function foo ()`

![eslint-config-standard-deviation][eslint-config-standard-deviation]
[eslint-config-standard-deviation]:./semicolon.jpg

[standard]: https://github.com/feross/eslint-config-standard

## Installation

### npm
```bash
npm install eslint-config-standard-deviation --save-dev
```

#### WITH dependencies installation
```bash
npm install eslint babel-eslint eslint-config-standard
npm install eslint-config-standard-react eslint-plugin-react eslint-plugin-promise eslint-plugin-standard --save-dev
```

#### OR add easily to projects using [eslint-modules-standard-deviation](https://github.com/bySabi/eslint-modules-standard-deviation)
```bash
npm install eslint eslint-modules-standard-deviation --save-dev
```
##### Works only in `npm 3` and beyond environments

## Usage
Add `extends` to project `.eslintrc`
```json
{
  "extends": ["standard-deviation"]
}
```
Add scripts to `package.json`
```json
"scripts": {
  "lint": "eslint . --ext .js,.jsx",
  "testonly": "echo \"Error: no test specified\" && exit 1",
  "test": "npm run lint && npm run testonly"
}
```

### [optional] enable/disable [eslint rules](http://eslint.org/docs/rules/)
```json
{
  "extends": ["standard-deviation"],
  "rules": {
    "space-before-function-paren": ["2", "always"]
  }
}
```

## for Javascript `ES5` only, use
* [eslint-config-standard-deviation--es5](https://github.com/bySabi/eslint-config-standard-deviation--es5)
* [eslint-modules-standard-deviation--es5](https://github.com/bySabi/eslint-modules-standard-deviation--es5)

## Projects using `eslint-config-standard-deviation`
* [react-scrollchor](https://github.com/bySabi/react-scrollchor)
* [react-scrollaware](https://github.com/bySabi/react-scrollaware)

## Contributing

* Documentation improvement
* Feel free to send any PR

## License

[ISC][isc-license]

[isc-license]:./LICENSE
