---
description: Frequently Asked Questions
---

# FAQ

## What Wallet Connection Methods Are Available?

The only supported wallet connection method is via the Terra Chrome Extension. The Ledger hardware wallet is supported through the Terra Chrome Extension.

## Are There Plans To Implement Terra Station Mobile Support?

There are no plans to implement Terra Station Mobile support due to limitations of the Terra Station Mobile app.

Some context: When linking a wallet to your discord account, you are prompted to sign a dummy transaction with your wallet. This transaction is never sent to the blockchain but is instead sent to the Lunar Assistant backend and used to prove that you own your wallet (only those with ownership of their wallet are able to sign transactions). By sending it to the backend instead of posting it on-chain, we can avoid incurring any fees for the user linking their wallet via Lunar Assistant.

Unfortunately, Terra Station Mobile does not support signing dummy transactions; it only supports posting transactions to the blockchain. This means that if Lunar Assistant were to support mobile, it would mean that users would incur a transaction fee when linking their wallets via Lunar Assistant.

If the demand for mobile support remains high despite the transaction fees that would be required by users on mobile, we may consider supporting it in the future. For now though, given that everyone has the Terra Chrome Extension and linking a wallet is a one time process, there are no plans to support mobile.

