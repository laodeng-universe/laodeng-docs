# Deploy Smart Contracts

LAODENG Universe is EVM-compatible and supports Ethereum-style smart contracts.

## Requirements

Before deployment, prepare:

- An EVM-compatible development environment
- A wallet connected to LAODENG Universe
- Enough LDU to pay deployment gas fees
- A reviewed and tested smart contract

## Official Network Configuration

| Setting | Value |
|---|---|
| RPC URL | https://rpc.laodeng.org |
| Chain ID | 20260001 |
| Native Symbol | LDU |
| Block Explorer | https://scan.laodeng.org |

## Recommended Workflow

1. Compile the contract locally.
2. Run automated tests.
3. Review permissions and owner functions.
4. Estimate deployment gas.
5. Confirm the wallet is connected to LAODENG Universe.
6. Deploy the contract.
7. Save the contract address and transaction hash.
8. Verify the deployment through the official block explorer.

## Security Checklist

Before publishing a contract:

- Review access-control functions.
- Confirm minting and upgrade permissions.
- Test pause and emergency functions.
- Avoid exposing private keys.
- Use a dedicated deployment wallet.
- Consider an independent security review for contracts handling valuable assets.

## Disclaimer

Smart contract deployment is irreversible once confirmed.

Developers are responsible for testing, auditing, and securely managing deployment credentials.
