After implement the function to get the jsx of element. We need some packages to configure the react. 
```
pnpm i -D -w rollup-plugin-generate-package-json
pnpm i -D -w rollup-plugin-typescript2
pnpm i -D -w @rollup/plugin-commonjs
pnpm i -D -w rimraf
```
- `rollup-plugin-generate-package-json`: Used to generate `package.json` files.
- `rollup-plugin-typescript2`: Used to complie Typescript
- `@rollup/plugin-commonjs`: Used to convert commonJS modules to ES modules for packaging in Rollup. CommonJS is a module specification for executing JS code outside of the browser, and Rollup only supports ES modules by default.
- `rimraf`: Used to delete the previous package products.
