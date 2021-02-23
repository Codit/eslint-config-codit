# Version 1.x.x

Documentation for all versions below 2.x.x
Version 1.x.x has support for FlowType & Lodash which we are no longer supporting @ Codit and moving forward with version 2.x.x

## Usage

### Installation

```
yarn add eslint-config-unbrace eslint@^6.8.0 --dev
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
