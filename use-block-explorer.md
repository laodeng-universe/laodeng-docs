# Use the LAODENG Universe Block Explorer

This guide explains how to use the official LAODENG Universe block explorer to view transactions, wallet addresses, blocks, and network activity.

## Official Block Explorer

Use the official explorer:

`https://scan.laodeng.org`

Always verify that the domain is exactly:

`scan.laodeng.org`

## Search for a Transaction

1. Open the official block explorer.
2. Copy the transaction hash from your wallet.
3. Paste the transaction hash into the search bar.
4. Open the matching result.

The transaction page may display:

- Transaction status
- Transaction hash
- Block number
- Sender address
- Recipient address
- Transferred amount
- Gas used
- Network fee
- Confirmation time

## Search for a Wallet Address

1. Copy the public wallet address.
2. Paste it into the explorer search bar.
3. Open the address page.

The address page may display:

- Current LDU balance
- Transaction history
- Sent transactions
- Received transactions
- Contract interactions
- Token activity

Only public blockchain information is visible. Private keys and seed phrases are never shown on a block explorer.

## Search for a Block

1. Copy or enter a block number.
2. Paste it into the search bar.
3. Open the block page.

The block page may display:

- Block number
- Block hash
- Timestamp
- Validator or miner information
- Number of transactions
- Gas usage
- Parent block hash

## Transaction Status

Common transaction statuses include:

- **Success** — The transaction was confirmed and executed.
- **Pending** — The transaction has not yet been confirmed.
- **Failed** — The transaction was included in a block but execution failed.

A failed transaction may still consume a network fee.

## Verify Transfer Details

Before considering a transfer complete, verify:

- The transaction status is **Success**
- The recipient address is correct
- The transferred amount is correct
- The transaction is on **LAODENG Universe**
- The Chain ID is `20260001`

## Security Warning

Do not trust links sent by unknown users.

Only use the official explorer published through:

- https://laodeng.org
- https://github.com/laodeng-universe

A block explorer will never ask for your private key or seed phrase.
