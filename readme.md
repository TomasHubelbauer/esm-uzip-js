# ESM UZIP.js

![](https://github.com/tomashubelbauer/esm-uzip-js/workflows/.github/workflows/update.yml/badge.svg)

This is the [UZIP.js](https://github.com/photopea/UZIP.js) library provided as an ESM package.

## Usage

```
import UZIP from 'https://tomashubelbauer.github.io/esm-uzip-js/index.js';
// Usage as per https://github.com/photopea/UZIP.js#interface
```

## How Does It Work / Is It Stale?

This repository updates its UZIP.js submodule automatically every day and while doing that
copies the `UZIP.js` file from it to `index.js` appending `export default UZIP;` and the
current date.

A GitHub Actions workflow is used to accomplish that:
[`.github/worflows/update.yml`](.github/worflows/update.yml)

GitHub Pages are used to serve the contents of the repository, this is better than using
the *Raw* option on GitHub, because the file also has a correct MIME type and thus can be
used as an ESM module.
