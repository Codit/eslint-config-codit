# Unbrace ESLint Config

_An fair-minded way to reduce noise in Javascript_

The goal of this package is to have a consistent coding style across multiple files / projects while not being overly strict.

>Note: We also use [Prettier](https://github.com/prettier/prettier) as a precommit hook, so indentation etc. is not really a part of the configuration. If you do need it, you can always override the configuration. See [eslint-indent](https://eslint.org/docs/rules/indent) for more information.

## Usage

### Installation
```
yarn add eslint-config-unbrace
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

MIT