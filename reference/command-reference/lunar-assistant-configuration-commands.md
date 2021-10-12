# Lunar Assistant Configuration Commands

## Configuring Lunar Assistant Rules

Command group for configuring the rules which grant roles based on wallet holdings. Useful for creating private channels that only those with certain wallet holdings have access to, and for letting users show off their wallets via roles.

{% hint style="info" %}
The below commands are displayed like api endpoints, but really they are discord slash commands accessible from discord servers with the Lunar Assistant. The below commands are only usable by those with the `Lunar Commander` role. The `Lunar Commander` role is created in your discord server when you add the Lunar Assistant bot.
{% endhint %}

{% swagger method="get" path="lunar-configure add-rule" baseUrl="/" summary="" %}
{% swagger-description %}
Adds a rule for granting a role to users. When a user's wallet meets the conditions of the rule, they will be granted the relevant role.
{% endswagger-description %}

{% swagger-parameter in="body" name="nft-address" type="string" required="true" %}
The contract address against which to check for nft ownership
{% endswagger-parameter %}

{% swagger-parameter in="body" name="role" type="Role" required="true" %}
The role to give to users which meet this rule.
{% endswagger-parameter %}

{% swagger-parameter in="body" name="quantity" type="number" %}
The quantity of matching nfts that a user must hold in order to meet the rule. 1 by default.
{% endswagger-parameter %}

{% swagger-parameter in="body" name="token-ids" type="string" %}
A list of token ids that the rule is restricted to. All tokens by default.
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="get" path="lunar-configure view-rules" baseUrl="/" summary="" %}
{% swagger-description %}
View the rules currently configured for the server.
{% endswagger-description %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="get" path="lunar-configure remove-rule" baseUrl="/" summary="" %}
{% swagger-description %}
Remove a rule based on its index in the output of 

`/view-rules`

.
{% endswagger-description %}

{% swagger-parameter in="body" name="rule-number" type="number" required="true" %}
The index of  the rule to remove.
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

## Lunar Assistant Configuration in Action

To see lunar assistant configuration commands in action, see the following page:

{% content-ref url="../../admin-guide/discord-bot-setup-quick-start/token-permissioned-roles.md" %}
[token-permissioned-roles.md](../../admin-guide/discord-bot-setup-quick-start/token-permissioned-roles.md)
{% endcontent-ref %}

