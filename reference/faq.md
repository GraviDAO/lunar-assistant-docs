---
description: Frequently Asked Questions
---

# FAQ

## What Wallet Connection Methods Are Available?

The only supported wallet connection method is via the Terra Chrome Extension. The Ledger hardware wallet is supported through the Terra Chrome Extension.

## Are There Plans To Implement Terra Station Mobile Support?

Short Answer: There are no plans to implement Terra Station Mobile support due to limitations of the Terra Station Mobile app.

Long Answer: When linking a wallet to your discord account, you are prompted to sign a dummy transaction with your wallet. This transaction is never sent to the blockchain but is instead sent to the Lunar Assistant backend and used to prove that you own your wallet (only those with ownership of their wallet are able to sign transactions). By sending it to the backend instead of posting it on-chain, we can avoid incurring any fees for the user linking their wallet via Lunar Assistant.

Unfortunately, Terra Station Mobile does not support signing dummy transactions; it only supports posting transactions to the blockchain. This means that if Lunar Assistant were to support mobile, it would mean that users would incur a transaction fee when linking their wallets via Lunar Assistant.

If the demand for mobile support remains high despite the transaction fees that would be required by users on mobile, we may consider supporting it in the future. For now though, given that everyone has the Terra Chrome Extension and linking a wallet is a one time process, there are no plans to support mobile.

## Are NFTs listed on marketplaces considered during role assignment?

Lunar Assistant supports NFTs listed on the following marketplaces:

* RandomEarth
* Knowhere.art (Coming soon)

This means that NFTs listed on the above marketplaces will be considered during role assignment, and that NFTs listed on other marketplaces will not be considering during role assignment.

These marketplaces are supported because of contributions by the marketplace teams. For every marketplace that the lunar assistant supports, it must be done in collaboration with the marketplace's team.

If you see a marketplace missing from the above list, feel free to reach out so that we can get a collaboration started with the missing marketplace.

## Where are the saved wallet addresses stored?

The mapping between discord user accounts and terra wallet addresses is stored in a centralized database that only Lunar Assistant maintainers have access to. Lunar Assistant will never share or sell any data, and only looks at the database for debugging purposes.

\


