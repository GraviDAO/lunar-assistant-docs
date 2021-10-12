---
description: More info on the architecture powering Lunar Assistant.
---

# Architecture

## Lunar Assistant Discord Bot Command Handler

The Lunar Assistant Discord Bot is run on a digital ocean droplet.

## Lunar Assistant Wallet Holdings Tracker

There are a few processes involved with keeping discord user roles in sync with their wallet addresses.

### Watching All Transactions

The Lunar Assistant watches all transactions and filters for those involving NFT transfers. Whenever an NFT transfer takes place, the Lunar Assistant checks whether or not any of the involved wallets are connected to a Discord account. If so, then the given user's Discord roles are updated with respect to their new wallet holdings. This allows for almost realtime role updates.

### Cron Job

A cron job runs once a day which syncs every registered Discord user's roles with their wallet holdings. The point of this is to handle edge cases where transactions are missed in the "Watching All Transactions" approach.

```
  // read all users from firestore
  // read all serverConfigs from firestore
  // for each user in users (in memory)
  //   for each serverConfig in serverConfigs (in memory)
  //     check if the user is in the server (in memory), if so:
  //       for each rule in serverConfig (in memory)
  //         query the user tokens relevant to the rule (cache if possible)
  //         update user's discord roles according to rule
  //         save the user's discord roles to firestore
```

### On User Wallet Address Update

Each time a user updates their linked wallet address, that user's Discord roles are synced with their new wallet holdings.

