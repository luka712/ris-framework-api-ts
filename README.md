# ris-framework-api

TypeScript interfaces for the ris framework, generated from `RisFramework.API.csproj`. Version 1.0.0.

This package is the type surface. It does not ship a renderer. `IFramework` is the root: graphics device, renderer, pipelines, buffers, textures, cameras, meshes, materials, content, input, window, and time. `ktx2Factory` is present only when KTX2 is requested, and that type comes from `ris-ktx2-api`.

## Install

```sh
npm install ris-framework-api
```

The package is ESM only. `package.json` `exports` resolves JavaScript to `dist/index.js` and types to `dist/index.d.ts`. Runtime dependencies are `gl-matrix` and `ris-ktx2-api`.

## Exports

Everything is exported from the package root, including `IFramework` and `IFrameworkConfig`.

## Release

`development` publishes `<version>-dev.<run>` on the npm dist-tag `next`. `main` publishes `<version>` on `latest` when that version is not already on npm, then tags `v<version>` and opens a GitHub release. See `CONTRIBUTING.md`.
