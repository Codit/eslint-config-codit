# Unbrace ESLint Config

_A fair-minded way to reduce noise in Javascript_

The goal of this package is to have a consistent coding style across multiple files / projects while not being overly strict and have a minimal setup procedure.

The package contains our ESLint rules, including ES6, React, FlowType & Lodash and requires `eslint@^4.0.0`.

>Note: We also use [Prettier](https://github.com/prettier/prettier) as a precommit hook, together with their [eslint-config-prettier](https://github.com/prettier/eslint-config-prettier), so we might not meet your standards on indentation etc. If you do need it, you can always override the configuration with extra rules. See  [Configuring ESLint](https://eslint.org/docs/user-guide/configuring) for more information.

## Usage

### Installation
```
yarn add eslint-config-unbrace --dev
```

### Configuration
```
  "eslintConfig": {
    "extends": [
      "unbrace"
    ]
  }
```

## License

[MIT](LICENSE)