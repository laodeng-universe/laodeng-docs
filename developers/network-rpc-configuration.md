# Network and RPC Configuration

This document provides the official LAODENG Universe mainnet parameters for developers.

## Mainnet Parameters

| Setting | Value |
|---|---|
| Network Name | LAODENG Universe |
| Chain ID | 20260001 |
| Hex Chain ID | 0x13524a1 |
| Native Symbol | LDU |
| Decimals | 18 |
| RPC URL | https://rpc.laodeng.org |
| Block Explorer | https://scan.laodeng.org |

## JSON-RPC Example

```bash
curl -X POST https://rpc.laodeng.org \
  -H "Content-Type: application/json" \
  --data '{"jsonrpc":"2.0","method":"eth_chainId","params":[],"id":1}'
```

The expected Chain ID response corresponds to:

`0x13524a1`

## JavaScript Provider Example

```javascript
import { JsonRpcProvider } from "ethers";

const provider = new JsonRpcProvider(
  "https://rpc.laodeng.org",
  {
    name: "LAODENG Universe",
    chainId: 20260001
  }
);

const blockNumber = await provider.getBlockNumber();
console.log(blockNumber);
```

## Important Notes

- Always verify the Chain ID before submitting transactions.
- Do not hard-code private keys in source code.
- Use environment variables for sensitive configuration.
- Applications should handle RPC errors and temporary connection failures.
