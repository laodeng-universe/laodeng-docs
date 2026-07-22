# Web3 Application Integration

This guide provides basic information for connecting a Web3 application to LAODENG Universe.

## Network Parameters

| Setting | Value |
|---|---|
| Network Name | LAODENG Universe |
| RPC URL | https://rpc.laodeng.org |
| Chain ID | 20260001 |
| Hex Chain ID | 0x13524a1 |
| Native Symbol | LDU |
| Decimals | 18 |
| Block Explorer | https://scan.laodeng.org |

## Add Network with an EIP-1193 Wallet

```javascript
const LAODENG_UNIVERSE = {
  chainId: "0x13524a1",
  chainName: "LAODENG Universe",
  nativeCurrency: {
    name: "LDU",
    symbol: "LDU",
    decimals: 18
  },
  rpcUrls: ["https://rpc.laodeng.org"],
  blockExplorerUrls: ["https://scan.laodeng.org"]
};

await window.ethereum.request({
  method: "wallet_addEthereumChain",
  params: [LAODENG_UNIVERSE]
});
```

## Switch Network

```javascript
await window.ethereum.request({
  method: "wallet_switchEthereumChain",
  params: [{ chainId: "0x13524a1" }]
});
```

## Verify the Connected Network

```javascript
const chainId = await window.ethereum.request({
  method: "eth_chainId"
});

if (chainId.toLowerCase() !== "0x13524a1") {
  throw new Error("Please switch to LAODENG Universe.");
}
```

## Application Safety

- Never request a user's seed phrase or private key.
- Display transaction details before requesting confirmation.
- Validate the connected Chain ID.
- Handle rejected wallet requests.
- Use the official RPC and explorer URLs.
