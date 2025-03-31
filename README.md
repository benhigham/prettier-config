# `@benhigham/prettier-config`

[![npm version](https://img.shields.io/npm/v/@benhigham/prettier-config.svg)](https://www.npmjs.com/package/@benhigham/prettier-config)
[![npm downloads](https://img.shields.io/npm/dm/@benhigham/prettier-config.svg)](https://www.npmjs.com/package/@benhigham/prettier-config)
[![License](https://img.shields.io/github/license/benhigham/prettier-config)](LICENSE.md)

My personal [Prettier](https://prettier.io) configuration, designed to enforce consistent code formatting across my JavaScript and TypeScript projects.

## Features

- Sensible defaults for modern JavaScript/TypeScript development
- Ensures consistent formatting across different IDEs and editors
- Optimized for readability and maintainability
- Compatible with Prettier v3

## Installation

```sh
# npm
npm install --save-dev @benhigham/prettier-config

# yarn
yarn add --dev @benhigham/prettier-config

# pnpm
pnpm add --save-dev @benhigham/prettier-config
```

## Usage

### Method 1: Use in `package.json` (recommended)

```jsonc
{
  // ...
  "prettier": "@benhigham/prettier-config",
}
```

### Method 2: Use in `prettier.config.js`

If you need to extend the configuration:

```js
import benhighamPrettierConfig from '@benhigham/prettier-config';

/**
 * @type {import('prettier').Config}
 */
const config = {
  ...benhighamPrettierConfig,
  // your overrides here
};

export default config;
```

### Method 3: Use in `.prettierrc`

```json
"@benhigham/prettier-config"
```

## Requirements

- Node.js 18.20.x or higher
- [Prettier](https://prettier.io/) 3.x

## License

This project is licensed under the [MIT License](LICENSE.md).
