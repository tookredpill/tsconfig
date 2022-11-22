# @tookredpill/tsconfig

Shared TypeScript config for my projects.

## Install

```sh
yarn add -D @tookredpill/tsconfig
```

## Usage

Create a `tsconfig.json` file in your project and extend it with one of the available configs.

### Vite + React

```json
{
  "extends": "@tookredpill/tsconfig/configs/vite.json",
  "compilerOptions": {
    "jsx": "react-jsx"
  }
}
```

### Vite + Solid

```json
{
  "extends": "@tookredpill/tsconfig/configs/vite.json",
  "compilerOptions": {
    "jsx": "preserve",
    "jsxImportSource": "solid-js"
  }
}
```

### Node 16

```json
{
  "extends": "@tookredpill/tsconfig/configs/base.json",
  "compilerOptions": {
    "target": "ES2021",
    "module": "ES2022",
    "lib": ["ES2021"],
    "outDir": "dist"
  }
}
```

## License

[MIT](./LICENSE)
