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

`options.js` populates the options page, accessible through the gear icon at the lower left.

`receiveBTC.js` populates the balance (and its value in USD) for the selected currency.

`register.js` populates the registration page.

`send.js` populates the Send page for Guld transactions.

## `/js/vendor` files

This folder contains supporting libraries. We are using libraries from the following projects (descriptions are from each project's page):

- [BrowserFS](https://github.com/jvilk/BrowserFS) _is an in-browser filesystem that emulates the Node JS filesystem API and supports storing and retrieving files from various backends._

- [Decimal](https://github.com/MikeMcl/decimal.js) is _An arbitrary-precision Decimal type for JavaScript_.

- [EventEmitter](https://github.com/Olical/EventEmitter) is _Evented JavaScript for the browser_.

- [GitHub.js](http://github-tools.github.io/github/) is _a javascript library that makes it easy to interact with GitHub’s REST API in Node and in the browser._

- [Highland](http://github.com/caolan/highland) is a _high-level streams library._

- Isomorphic-Git is 

- Ledger-CLI

- Odometer

- OpenPGP

- ParaParse

- QRCode

We are also using a pair of libraries from the Guld project: `guld-lib` and `ledger-types`.

> **TODO** What should we link to for the Guld libraries?
