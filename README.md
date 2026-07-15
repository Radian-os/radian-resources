# Radian Resources

An npm monorepo for static design assets maintained by Radian OS. Each asset
collection is published as a public package under the `@radianos` scope and can
be consumed directly from npm or a CDN such as jsDelivr.

## Packages

- `@radianos/avatars` — transparent PNG avatars
- `@radianos/brand-logos` — brand logo SVGs
- `@radianos/country-flags` — country flag SVGs
- `@radianos/file-icons` — file type SVG icons

## Install

```sh
pnpm install
```

## Publish

Authenticate with npm, then publish every workspace package:

```sh
pnpm publish:packages
```

Assets are available from each package's `src` directory. For example:

```text
https://cdn.jsdelivr.net/npm/@radianos/avatars@1.0.0/src/1.png
```
