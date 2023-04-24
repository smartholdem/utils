# Utilities

## Caveats

-   The native `map`, `filter`, `reduce` and `forEach` will generally be faster when used on arrays that contain nothing but numerical values.
-   If you plan to use `formatCurrency` method with node.js for anything else then the `en-US` locale you'll have to make sure to properly setup https://github.com/unicode-org/full-icu-npm as node.js itself only ships with the `en-US` locale by default unless specifically build with more locales.
-   Do not use the `is*` methods of this package inside the [Node.js VM](https://nodejs.org/api/vm.html) as the results could be misleading.
-   The `pluralize` method does not support irregular plurals. Check [blakeembrey/pluralize](https://github.com/blakeembrey/pluralize) if you need support for those.

## Installation

### npm

```sh
npm install @smartholdem/utils
```

### yarn

```sh
yarn add @smartholdem/utils
```

### pnpm

```sh
pnpm add @smartholdem/utils
```

## Test

### npm

```sh
npm run test -- --coverage
```

### yarn

```sh
yarn test --coverage
```

### pnpm

```sh
pnpm run test -- --coverage
```

## Benchmark

### Clone

```sh
git clone git@github.com:SmartHoldem/utils.git
```

### Run

#### npm

```sh
npm install
npm run bench
```

#### yarn

```sh
yarn install
yarn bench
```

#### pnpm

```sh
pnpm install
pnpm run bench
```
