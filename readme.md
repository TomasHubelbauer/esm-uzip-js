# ESM UZIP.js

This is the [UZIP.js](https://github.com/photopea/UZIP.js) library provided as an ESM package.

## Usage

```
import UZIP from 'https://tomashubelbauer.github.io/esm-uzip-js/index.js';
// Usage as per https://github.com/photopea/UZIP.js#interface
```

## Stale?

The UZIP.js submodule and the `index.js` file which is created by taking the `UZIP.js` file
from the submodule and appending `export default UZIP;` to it are both updated daily using a
GitHub Actions workflow script found in
[`.github/worflows/update.yml`](.github/worflows/update.yml).

## To-Do

### Ensure not enqueing GitHub Pages build explicitly still serves updated `index.js`
