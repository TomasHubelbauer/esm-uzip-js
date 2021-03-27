# ESM UZIP.js

![](https://github.com/tomashubelbauer/esm-uzip-js/workflows/.github/workflows/update.yml/badge.svg)

This is the [UZIP.js](https://github.com/photopea/UZIP.js) library provided as
an ES module.

## Usage

```
import UZIP from 'https://tomashubelbauer.github.io/esm-uzip-js/index.js';
// Usage as per https://github.com/photopea/UZIP.js#interface
```

## How Does It Work / Is It Stale?

This repository updates its UZIP.js submodule automatically every day and while
doing that copies the `UZIP.js` file from it to `index.js` appending
`export default UZIP;` to make it a valid ES module.

A GitHub Actions workflow is used to accomplish that:
[`.github/worflows/update.yml`](.github/workflows/update.yml)

You can check it to see when it last run as well as click through the submodule
to the UZIP repository to see that the submodule is up to date with that repo.

GitHub Pages are used to serve the contents of the repository, this is better
than using the *Raw* option on GitHub, because the file also has a correct MIME
type and thus can be used as an ESM module.

## To-Do

### Purge the timestamp-only commits from the history

I've rethought adding them and they have polluted the history somewhat.
