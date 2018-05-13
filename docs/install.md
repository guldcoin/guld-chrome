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
- Chrome or Chromium
 ([chrome](https://www.google.com/chrome))
 ([chromium windows](https://chromium.woolyss.com/download/#windows))
 ([chromium mac](https://chromium.woolyss.com/download/#mac))
 ([chromium linux](https://chromium.woolyss.com/download/#linux))
- an Internet connection

<p style="color:red"><b>NEED HELP HERE!</b> What are the minimum Python and Chrome versions we should be requiring?</p>

## Installation

Once your system meets the minimum requirements, you can install the various components: the `ledger-cli` application, our `ledger-native` bindings, and finally the Chrome extensions themselves.

### Installing ledger-cli

The first package you need to install is `ledger-cli`, the command-line based accounting system. This allows the extensions to interact with the Guld ledger.

#### On macOS

Using the [Brew](https://docs.brew.sh/Installation) package manager, run the following command from a Terminal window:

```bash
brew install ledger
```

#### On Linux

The [ledger download page](https://www.ledger-cli.org/download.html) has links to `ledger` versions for several linux distributions.

**Note!** We only support ledger 3.1.1 and later. As of this writing, the *Slackware*, *CentOS*, and *OpenSUSE* packages were out of date, and may not work correctly with our extensions.

#### On Windows

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

1. Double-click the `install_host.bat` script to run it.

1. This script installs the native messaging host for the current user, by creating a registry key called `HKEY_CURRENT_USER\SOFTWARE\Google\Chrome\NativeMessagingHosts\com.guld.ledger` and setting its value to the full path to `com.guld.ledger-win.json`.

### Install the Chrome extension

Forthcoming...

#### Extension Setup Steps

Forthcoming...

Setup steps for each chrome app/extension

#### Guld Wallet

Forthcoming...

#### Guld Games

Forthcoming...
