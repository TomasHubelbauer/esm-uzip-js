# ESM UZIP.js

This is the [UZIP.js](https://github.com/photopea/UZIP.js) library provided as an ESM package.

## Usage

```
import UZIP from 'https://tomashubelbauer.github.io/esm-uzip-js/UZIP.js/UZIP.js';
// Usage as per https://github.com/photopea/UZIP.js#interface
```

## Stale?

As of now, the UZIP.js library is added as a submodule and updating it is done manually by
updating the submodule. This reflects on the GitHub Pages site from which the ESM library
is being referenced.

In the futute, I plan on introducing a GitHub Actions workflow which either automatically
updates the submodule daily or notifies me first so that I can consider the changes and
update myself.

## To-Do

### Develop a GitHub Actions workflow to update the UZIP.js Git submodule daily

### Copy `UZIP.js` to the root and add the `export default UZIP` line to it to make it ESM

Right now I'm just hosting the file using my GitHub Pages, but it is not an ESM module yet.
It looks like it will be better to not use the submodule and just clone, edit and commit
the changed version of `UZIP.js` but I kinda like how the submodule immediately shows what
version of UZIP.js is being used so I might keep using the submodule and just add UZIP.js
to the root alongside of it with the only patch being the export line.
