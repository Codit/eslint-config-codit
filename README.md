# Unbrace ESLint Config

_A fair-minded way to reduce noise in Javascript_

The goal of this package is to have a consistent coding style across multiple files / projects while not being overly strict and have a minimal setup procedure.

The package contains our ESLint rules, including ES6, React, TypeScript, FlowType & Lodash.

> Note: We also use [Prettier](https://github.com/prettier/prettier) as a precommit hook, together with their [eslint-config-prettier](https://github.com/prettier/eslint-config-prettier), so we might not meet your standards on indentation etc. If you do need it, you can always override the configuration with extra rules. See [Configuring ESLint](https://eslint.org/docs/user-guide/configuring) for more information.

## Usage

### Installation

```
yarn add eslint-config-unbrace --dev
```

Install dependencies. ESLint plugins [must also be installed](https://github.com/eslint/rfcs/pull/5).

```
yarn add -D eslint-plugin-babel@^5.3.0 eslint-plugin-filenames@^1.3.2 eslint-plugin-import@^2.19.1 eslint-plugin-promise@^4.2.1 eslint-plugin-react@^7.17.0 eslint-config-prettier@^6.9.0
```

### Configuration

The following configuration contains a setup for ES6, React, TypeScript & Prettier

```
  "eslintConfig": {
    "extends": [
      "unbrace"
    ]
  }
```

Or if you want to take more control or don't use TypeScript, you can also extend the packages as follows (make sure to also install the correct dependencies, FlowType & Lodash f.e. are not listed in the step above):

```
"eslintConfig": {
    "extends": [
      "unbrace/core",
      "unbrace/flowtype",
      "unbrace/lodash",
      "unbrace/react"
    ]
  }

// or

"eslintConfig": {
    "extends": [
      "unbrace/core",
      "unbrace/es5"
    ]
  }
```

## License

[MIT](LICENSE)
