# User Commands

## Lunar Link

Allows a user to link a wallet to their discord account. Upon using `/lunar-link`, the user will be sent a link to the lunar assistant website from which they can sign a transaction that proves ownership of the wallet they are registering.

For now a user can only have a single wallet registered at a time. Running lunar-link multiple times will overwrite the users existing wallet.

Upon linking a new wallet, the user's roles are updated to reflect the contents of the new wallet.

{% hint style="info" %}
The below commands are displayed like api endpoints, but really they are discord slash commands accessible from discord servers with the Lunar Assistant.
{% endhint %}

{% swagger method="get" path="lunar-link" baseUrl="/" summary="" %}
{% swagger-description %}
Replies to the user with a link that can be used to link a wallet address with their discord account.
{% endswagger-description %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

## Lunar View Roles

Forces a role update based on the contents of a user's linked wallet, then displays the roles that a user is granted across all Discord Servers that they are a part of with Lunar Assistant configured.

{% swagger method="get" path="lunar-view-roles" baseUrl="/" summary="" %}
{% swagger-description %}
Forces a role update based on the contents of a user's linked wallet, then displays the roles that a user is granted across all Discord Servers that they are a part of with Lunar Assistant configured.
{% endswagger-description %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

## Lunar View Wallet

Displays the wallet a user has linked to their account (only visible to the user who sent the command).

{% swagger method="get" path="lunar-view-wallet" baseUrl="/" summary="" %}
{% swagger-description %}
Displays the wallet a user has linked to their account (only visible to the user who sent the command).
{% endswagger-description %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

## Lunar Disconnect Wallet

Disconnects the user's discord account from their wallet address. This will cause them to lose all roles that were previously granted to them by the Lunar Assistant.

{% swagger method="get" path="lunar-disconnect-wallet" baseUrl="/" summary="" %}
{% swagger-description %}
Disconnects the user's discord account from their wallet address. This will cause them to lose all roles that were previously granted to them by the Lunar Assistant.
{% endswagger-description %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}
