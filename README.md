# Codit ESLint Config

_A fair-minded way to reduce noise in Javascript_

The goal of this package is to have a consistent coding style across multiple files / projects while not being overly strict and have a minimal setup procedure.

The package contains our ESLint rules, including Next.js, ES6, React & TypeScript.

> Note: We also use [Prettier](https://github.com/prettier/prettier) and integrated [eslint-config-prettier](https://github.com/prettier/eslint-config-prettier) within this package, so we might not meet your standards on indentation etc. If needed, you can always override the configuration with extra rules. See [Configuring ESLint](https://eslint.org/docs/user-guide/configuring) for more information.

## Usage

### Installation

```
yarn add --dev @codit/eslint-config eslint@8.22.0
```

### Configuration

The following configuration contains a setup for Next.js, ES6, React, TypeScript & Prettier, add it to your `.eslintrc` file

```json
"extends": ["@codit"]
```

Or if you want to take more control or don't use TypeScript, you can also extend the packages as follows (make sure to also install the correct dependencies):

```javascript

"extends": [
  "@codit/eslint-config/core",
  "@codit/eslint-config/react"
]

// or

"extends": [
  "@codit/eslint-config/core",
  "@codit/eslint-config/next"
]
```

## Older versions

Documentation for older versions can be found in the docs folder:

- [Version 2.x.x](./docs/version-2.x.x.md)
- [Version 1.x.x](./docs/version-1.x.x.md)

## License

[MIT](LICENSE)
