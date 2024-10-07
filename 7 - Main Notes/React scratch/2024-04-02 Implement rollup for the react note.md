
After create rollup we have some of the package to install

```
pnpm i -D -w rollup-plugin-generate-package-json
pnpm i -D -w rollup-plugin-typescript2
pnpm i -D -w @rollup/plugin-commonjs
pnpm i -D -w rimraf
```
- `rollup-plugin-generate-package-json`:  used to generate `package.json` file
- `rollup-plugin-typescript2`: Used to complie Typescript
- `@rollup/plugin-commonjs`: Used to convert CommonJS modules into ES modules for packaging in Rollup. CommonJS is a module specification for executing JS code outside the browser, and Rollup only supports ES modules by default
- `rimraf`: Used to delete previous packaged products