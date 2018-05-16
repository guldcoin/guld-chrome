# Folder structure

The files that make up this Chrome extension are organized into several folders:

## Root-level files

`.eslintrc.json` sets up behaviours for the [`eslint`](https://eslint.org/) JavaScript linter. **omit from the distribution??**

`.gitignore` lists file names and patterns that Git should silently omit from its operations. Refer to the [Git documentation](https://www.git-scm.com/docs/gitignore) for details.

`LICENSE` is the extension's MIT-style software license.

`manifest.json` provides information about the extension to the Chrome browser. Refer to the [Chrome developer docs](https://developer.chrome.com/extensions/manifest) for more details.

`package.json` is the general NPM package manifest. Refer to the [NPM developer docs](https://docs.npmjs.com/files/package.json) for details.

`package-lock.json` records exactly which NPM package versions used to create the current distribution. Refer to the [NPM developer docs](https://docs.npmjs.com/files/package-lock.json) for details.

`README.md` is the overview document for the project.

## `/css` files

`style.css` is the single CSS stylesheet for the extension's HTML pages.

## `/html` files

The files in the `/html` folder provide structure of the extension's HTML user interface. The files are documented individually.

Note that the content of these HTML files is manipulated by the scripts (in the `/js` folder) that define the extension's logic.

`main.html` is the base upon which the UI is built. The other files in this folder define supporting and related functionality.

## `/images` files

All of the images the extension uses are in the `/images` folder.

## `/js` files

The code that directly defines the extension's functionality is in the `/js` folder.

`main.js` defines the program logic, along with `util.js`. The other files in this folder provide supporting functionality.

`background.js` handles tasks including blocktree, PGP, GitHub, and browser-filesystem operations, and exposes the extension's API for use by other extensions.

`burn.js` provides functionality to burn GULD. **Not currently implemented**

`convert.js` provides functionality to convert between currencies. **Not currently implemented**

`deposit.js` provides functionality to deposit into the wallet. **Not currently implemented**

`fs.js` configures the browser-based filesystem.

`grant.js` provides functionality to grant GG. **Not currently implemented**

`options.js` ...

`receiveBTC.js` ...

`register.js` ...

`send.js` ...

## `/js/vendor` files

This folder contains supporting libraries.
