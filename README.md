# Flash USDT (USDT)

ERC20 token on Ethereum mainnet. Full interface clone of Tether's USDT
(name `Tether USD`, symbol `USDT`, 6 decimals) with a "flash" emission window:
the owner can mint temporary tokens that are burned after a deadline.

- **Contract:** `0x887A8891A307d62CcFe6e1E40bfc019aA80d4176`
- **Symbol / decimals:** USDT / 6
- **Verified:** Etherscan · Blockscout · Sourcify

## What is it

- `flashMint(to, amount, duration)` — mints tokens with an expiry window
- `flashBurn(from, amount)` — returns the flashed tokens (owner)
- `expireFlash(account)` — after the window, anyone can burn what remains
- `mint` / `burn` / `issue` / `redeem` — permanent supply, Tether-style
- `addBlackList` / `removeBlackList` / `destroyBlackFunds`, `pause` / `unpause`

Verified source is public on the explorers: the token behaves like USDT in
wallets (transferable, spendable P2P).

## Links

- Etherscan: https://etherscan.io/token/0x887A8891A307d62CcFe6e1E40bfc019aA80d4176
- Blockscout: https://eth.blockscout.com/address/0x887A8891A307d62CcFe6e1E40bfc019aA80d4176
- Sourcify: https://repo.sourcify.dev/1/0x887A8891A307d62CcFe6e1E40bfc019aA80d4176
