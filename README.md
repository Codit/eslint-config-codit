# Codit ESLint Config

_A fair-minded way to reduce noise in Javascript_

The goal of this package is to have a consistent coding style across multiple files / projects while not being overly strict and have a minimal setup procedure.

The package contains our ESLint rules, including ES6, React & TypeScript.

> Note: We also use [Prettier](https://github.com/prettier/prettier) and integrated [eslint-config-prettier](https://github.com/prettier/eslint-config-prettier) within this package, so we might not meet your standards on indentation etc. If needed, you can always override the configuration with extra rules. See [Configuring ESLint](https://eslint.org/docs/user-guide/configuring) for more information.

## Usage

### Installation

```
yarn add @codit/eslint-config eslint@^7.2.0 --dev
```

Install peer dependencies.

```
yarn add --dev @babel/eslint-plugin@^7.13.0 @typescript-eslint/eslint-plugin@^4.15.2 eslint@^7.20.0 eslint-plugin-filenames@^1.3.2 eslint-plugin-import@^2.22.1 eslint-plugin-promise@^4.3.1 eslint-plugin-react@^7.22.0 eslint-plugin-react-hooks@^4.2.0
```

### Configuration

The following configuration contains a setup for ES6, React, TypeScript & Prettier, add it to your `.eslintrc` file

```
"extends": ["@codit"]
```

Or if you want to take more control or don't use TypeScript, you can also extend the packages as follows (make sure to also install the correct dependencies):

```

"extends": [
  "@codit/eslint-config/core",
  "@codit/eslint-config/react"
]

// or

"extends": [
  "@codit/eslint-config/core",
  "@codit/eslint-config/es5"
]
```

## Older versions

Documentation for versions 1.x.x can be found in the docs folder:

- [Version 1.x.x](./docs/version-1.x.x.md)

## License

[MIT](LICENSE)
