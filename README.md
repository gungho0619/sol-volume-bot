# Solana Volume Bot

This repo serves to  help you achieve desired transaction volumes on the Solana blockchain. This powerful tool is perfect for users looking to manage multiple transactions effectively

## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

```
BOT_NAME = "YOUR_BOT_NAME_HERE"
AUTH_KEYPAIR_PATH = "YOUR_SOLANA_WALLET_KEY_PAIR_HERE"
RPC_URL = "YOUR_SOLANA_RPC_URL_HERE"
...
```
Please check more environment variables in `src/clients/config.ts`


## Run Locally

Clone the project

```bash
  git clone https://github.com/gungho0619/sol-volume-bot.git
```

Go to the project directory

```bash
  cd sol-volume-bot
```

Install dependencies

```bash
  npm install
```

Start the server

```bash
  npm run dev
```

## Execution Steps

Caution: Run all steps in order and do not create new keypairs unless you reclaim your SOL.

#### 1. Create New Keypairs

Create new keypairs for your volume transactions. This step is necessary if you want to ensure fresh keypairs.

#### 2. Distribute SOL/WSOL

Distribute SOL/WSOL to the keypairs.

- Gas Fees: The SOL you send here is ONLY FOR GAS FEES. It is recommended to send anywhere from 0.05 to 1 SOL.
- Volume Spam: This is the amount of SOL each keypair will use to volume spam and rotate. You can enter any custom amount to look natural.

#### 3. Start Volumn

Execute the volume bot to get your desired volume. It is recommended to set a timeout between swaps at around 3-10 seconds to look natural.

#### 4. Retrieve Funds

Retrieve all funds from the keypairs automatically. This step will retrieve all the WSOL and SOL you sent and send it to the wallet in the config file.

#### 5. Simulate Volume

Simulate all volume and calculate all Jito tip fees and Raydium 5bps fee to see EXACTLY how much you will spend to achieve the volume you want. This step ensures you know the exact costs involved.

#### 6. Check Balance

Check balances of keypairs you created.


## Badges

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/) [![GPLv3 License](https://img.shields.io/badge/License-Flamingo-red.svg)](https://opensource.org/licenses/)

## Authors

- [Flamingo](https://www.github.com/gungho0619)

## Feedback

If you have any feedback, please reach out to me via [mail](tzztson@gmail.com) or [telegram](https://t.me/gungho0619)
