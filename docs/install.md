# Guld Wallet/Guld Games App Installation

Instructions for how to install the GULD Wallet/Guld Games App

## Installation

### Pre-requirements

- python 2.7 or newer
- chrome 66 or newer

### Step1. Install **Python** 

Download the latest release for your operating system: https://www.python.org/downloads/ and then run the installation package

### Step 2. Install **ledger-cli** 

##### Mac:

Brew Install (Recommended): https://docs.brew.sh/Installation

After installing Brew run `brew install ledger` from the **terminal**

##### Linux: 

Various linux versions can be found here: https://www.ledger-cli.org/download.html

##### Windows: 

Download the latest binaries https://github.com/AlexanderAA/ledger_binaries_windows/raw/master/ledger_3.1.1_win_bin.zip and install `ledger.exe`

### Step 3. Install **ledger-native** bindings

Download or clone ledger-native: https://github.com/guldcoin/ledger-native

Open your favorite **terminal** and `cd` into the **ledger-native** directory

##### Mac/Linux: 

Run the `install_host.sh` script.

By default the host is installed only for the user who runs the script, but if you run it with admin privileges (i.e. `sudo install_host.sh`), then the host will be installed for all users. You can use `uninstall_host.sh` to uninstall the host.

##### Windows: 

Run `install_host.bat` script.

This script installs the native messaging host for the current user, by creating a registry key `HKEY_CURRENT_USER\SOFTWARE\Google\Chrome\NativeMessagingHosts\com.guld.ledger` and setting its default value to the full path to `com.guld.ledger-win.json .` If you want to install the native messaging host for all users, change HKCU to HKLM.

### Step 4. Install Chrome Extension

Download Chrome first if you don’t already have it

https://www.google.com/chrome/

### Extension Setup Steps

Setup steps for each chrome app/extension


#### Guld Wallet


#### Guld Games

