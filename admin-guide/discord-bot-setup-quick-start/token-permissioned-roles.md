---
description: Guide to setting up token permissioned roles.
---

# Token Permissioned Roles

When configuring token permissioned roles, the following commands are your friend:

## /lunar-configure add-rule

Use `/lunar-configure add-rule` to add a token permissioned role to your server. Each token permissioned role is composed of the following properties:

* nft-address (required) : The contract address against which to check for nft ownership
* role (required) : The role to give to users which meet this rule.
* quantity (optional, 1 by default) : The quantity of matching nfts that a user must hold in order to meet the rule.
* token-ids (optional, all by default) : A list of token ids that the rule is restricted to. This can be used to add nft trait based roles. Calculate the list of token ids specific to a trait (galactic glitch for example) and then pass these token ids in when creating a rule.

{% hint style="info" %}
Example: `/lunar-configure add-rule nft-address: terra103z9cnqm8psy0nyxqtugg6m7xnwvlkqdzm4s4k role: @Galactic Civilian`

This adds a rule which grants anybody with at least one galactic punk (the nft address points to the galactic punk contract) the role `Galactic Civilian`
{% endhint %}

![The output of running /lunar-configure add-rule](<../../.gitbook/assets/image (2).png>)

## /lunar-configure view-rules

Use `/lunar-configure view-rules` to view the rules currently configured for your server. Example response:

![The ouput of running /lunar-configure view-rules](../../.gitbook/assets/image.png)

## /lunar-configure remove-rule

Use `/lunar-configure remove-rule` to remove a previously added rule. Example response:

![The output of running /lunar-configure remove-rule](<../../.gitbook/assets/image (5).png>)

## Further Reading

To learn more about lunar assistant configuration commands, see the following reference:

{% content-ref url="../../reference/command-reference/lunar-assistant-configuration-commands.md" %}
[lunar-assistant-configuration-commands.md](../../reference/command-reference/lunar-assistant-configuration-commands.md)
{% endcontent-ref %}

