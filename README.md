# eslint-config-ariyalabs [![Build Status](https://travis-ci.org/ariyalabs/eslint-config-ariyalabs.svg?branch=master)](https://travis-ci.org/ariyalabs/eslint-config-ariyalabs)

> ESLint [shareable config](http://eslint.org/docs/developer-guide/shareable-configs.html)


## Installation

```
$ npm install --save-dev eslint eslint-config-ariyalabs
```


## Usage

Once the `eslint-config-ariyalabs` package is installed, you can use it by specifying `ariyalabs` in the [`extends`](http://eslint.org/docs/user-guide/configuring#extending-configuration-files) section of your [ESLint configuration](http://eslint.org/docs/user-guide/configuring).

```js
{
  "extends": "ariyalabs",
  "rules": {
    // Additional, per-project rules...
  }
}
```

### Using the `ariyalabs` config with `eslint:recommended`

There are several rules in the [`eslint:recommended` ruleset](http://eslint.org/docs/rules/) that you might want to override and enforce in your project.

To use AriyaLabs style in conjunction with ESLint's recommended rule set, extend them both, making sure to list `ariyalabs` last:

```js
{
  "extends": ["eslint:recommended", "ariyalabs"],
  "rules": {
    // Additional, per-project rules...
  }
}
```

To see how the `ariyalabs` config compares with `eslint:recommended`, refer to the [source code of `index.js`](https://github.com/ariyalabs/eslint-config-ariyalabs/blob/master/index.js), which lists every ESLint rule along with whether (and how) it is enforced by the `ariyalabs` config.


## License

Apache-2 © AriyaLabs
