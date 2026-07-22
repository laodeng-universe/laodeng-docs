# Understand LAODENG Universe Network Fees

LDU is the native asset of LAODENG Universe and is used to pay network transaction fees.

## What Is a Network Fee?

A network fee is the amount paid to process and confirm an operation on the blockchain.

Common operations that require a fee include:

- Sending LDU
- Deploying a smart contract
- Interacting with a smart contract
- Transferring tokens
- Using decentralized applications

## Gas

LAODENG Universe is EVM-compatible and uses the gas model.

The final fee depends on:

- Gas used by the transaction
- Gas price selected by the wallet
- Complexity of the operation
- Current network conditions

A simple LDU transfer normally uses less gas than a smart contract interaction.

## Before Sending a Transaction

Make sure your wallet has enough LDU for:

- The amount being transferred
- The estimated network fee

If the wallet does not contain enough LDU, the transaction cannot be submitted successfully.

## Failed Transactions

A failed transaction may still consume a network fee because validators processed the transaction before it failed.

Always review:

- Recipient address
- Selected network
- Transaction amount
- Estimated gas fee
- Smart contract permissions

## Verify Fees

Use the official block explorer to view the actual fee paid:

`https://scan.laodeng.org`

Never trust a website that asks for your private key or seed phrase to estimate a network fee.
