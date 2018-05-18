# Guld Wallet/Guld Games App Installation

This page describes how to install the GULD Wallet/Guld Games App.

## Before you install

Currently, these extensions run only on the following operating systems:

- macOS (10.12.x or later)
- Linux (kernel xxx or later, Ubuntu/Mint/Gentoo recommended)
- Windows (7 or later)

<p style="color:red"><b>NEED HELP HERE!</b> What are the minimum OS versions we should be requiring?</p>

In addition, you'll need:

- Python 2.7 or later ([download](https://www.python.org/downloads))
- Chrome ([chrome](https://www.google.com/chrome))
- or Chromium for [Windows](https://chromium.woolyss.com/download/#windows), [macOS](https://chromium.woolyss.com/download/#mac), or [Linux](https://chromium.woolyss.com/download/#linux)
- an Internet connection

<p style="color:red"><b>NEED HELP HERE!</b> What are the minimum Python and Chrome versions we should be requiring?</p>

## Installation

Once your system meets the minimum requirements, you can install the various components: the `ledger-cli` application, our `ledger-native` bindings, and finally the Chrome extensions themselves.

### Installing ledger-cli

The first package you need to install is `ledger-cli`, the command-line based accounting system. This allows the extensions to interact with the Guld ledger.

#### ledger-cli installation on macOS

Using the [Brew](https://brew.sh) package manager, run the following command from a Terminal window:

```bash
brew install ledger
```

#### ledger-cli installation on Linux

The [ledger download page](https://www.ledger-cli.org/download.html) has links to `ledger` versions for several linux distributions.

**Note!** We only support ledger 3.1.1 and later. As of this writing, the *Slackware*, *CentOS*, and *OpenSUSE* packages were out of date, and may not work correctly with our extensions.

#### ledger-cli installation on Windows

The [ledger download page](https://www.ledger-cli.org/download.html) has a link to a third-party binary download for Windows. Download and unzip `ledger_3.1.1_win_bin.zip`.

<p style="color:red"><b>NEED WINDOWS HELP HERE!</b> I'm not sure where the files should go... The binary unzips to a bunch of DLLs and a single executable. Seems like it ought to go into a folder of its own somewhere, but then we need to add instructions on adding that folder to the Windows path so the extension can find it.</p>

### Installing the ledger-native bindings

The `ledger-native` bindings allow the extensions to interact with the `ledger-cli` application. The bindings are necessary as browser-based extensions cannot interact directly with command lines.

#### On macOS and Linux

To install the ledger-native bindings on macOS or Linux:

1. Download (or clone, if you're handy with `git`) the [ledger-native](https://github.com/guldcoin/ledger-native) repository into your home directory, or another location if you'd prefer.

    **Note!** The next step assumes you placed the ledger-native files into your home directory. Adjust accordingly if you placed them elsewhere.

1. Open a shell window (such as Terminal on macOS) and issue the following commands:

    ```bash
    cd ledger-native

    ./install_host.sh
    ```

1. To uninstall the host, run `./uninstall_host.sh`.

#### On Windows

To install the ledger-native bindings on Windows:

1. Download (or clone, if you're handy with `git`) the [ledger-native](https://github.com/guldcoin/ledger-native) repository into your home directory, or another location if you'd prefer.

1. In an Explorer window, navigate to the `ledger-native` folder.

1. Double-click the `install_host.bat` script to install the native messaging host for the current Windows user.

### Install the Chrome extension

The extension will soon be available from the Google Play Store.

To install the extension directly from this Github repository, either download or clone the repository. Then, in Chrome:

1. Navigate to [chrome://extensions/](chrome://extensions/).

1. Turn on Developer Mode with the switch in the upper-right corner.

1. Click the `Load Unpacked` button.

1. Navigate to the location you downloaded or cloned the repository, and click Select.

    The extension's icon will show up on the Chrome toolbar, with a "WAIT" overlay. After a few minutes, the extension will finish its initial setup, and will be ready to use.

#### Extension Setup Steps

> **This section is incomplete...**

Once the extension has finished its initial setup, the "WAIT" overlay on its icon will disappear. Click the icon to get started!

#### Setting up Guld Wallet

> **This section is incomplete...**

Click the Guld Wallet icon on the Chrome toolbar to open the interface in a new tab. You'll be prompted to enter your Github credentials.

On the welcome screen, you can either **generate** a Guld identity, or **import** an existing identity. Identities are tied to PGP keys, so this step is actually generating a (or importing an existing, in the case of existing Guld users) PGP key.

To **generate a new Guld identity** and PGP key:

1. Select the "generate" radio button.

1. Choose a Guld username.

    > **TODO** Need guidelines on usernames.

1. Optionally, enter your name.

1. Enter your email address.

    Note that this email address will be publicly available in the ledger. Don't use an address you don't want to be made public!

1. Enter a strong passphrase for the new PGP key, and confirm it.

    Keep your passphrase stored securely! There is no way to recover a lost passphrase.

1. Click **Create** to create your new Guld identity and PGP key.

To **import an existing Guld identity** and PGP key:

> **TODO** it looks like the UI for this one is broken right now. Choosing import doesn't change the UI at all.

1. Select the "import" radio button.

1. ...

#### Setting up Guld Games

> **This section is forthcoming...**
