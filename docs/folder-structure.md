# Folder structure

The files that make up this Chrome extension are organized into several folders:

## Root-level files

`.eslintrc.json` sets up behaviours for the [`eslint`]() package, useful for development. **omit from the distribution??**

`.gitignore` lists file names and patterns that Git should silently omit from its operations. Refer to the [Git documentation](https://www.git-scm.com/docs/gitignore) for details.

`LICENSE` contains a copy of the extension's MIT-style software license.

`manifest.json` provides information about the extension to the Chrome browser. Refer to the [Chrome developer docs](https://developer.chrome.com/extensions/manifest) for more details.

`package-lock.json` records exactly which NPM package versions used to create the current distribution. Refer to the [NPM developer docs](https://docs.npmjs.com/files/package-lock.json) for details.

`package.json` is the general NPM package manifest. Refer to the [NPM developer docs](https://docs.npmjs.com/files/package.json) for details.

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

`background.js`

`burn.js`

`convert.js`

`deposit.js`

`fs.js`

`grant.js`

`options.js`

`receiveBTC.js`

`register.js`

`send.js`

## `/js/vendor` files

Contains supporting libraries.
