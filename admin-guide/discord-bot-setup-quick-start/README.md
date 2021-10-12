# Discord Bot Setup Quick Start

## 1. Create a Discord Server

You can use an existing server for which you are an admin, or use the following guide to create a new server: [https://support.discord.com/hc/en-us/articles/206143407](https://support.discord.com/hc/en-us/articles/206143407)

## 2. Add Lunar Assistant to your Discord Server

You can add Lunar Assistant to your Discord Server by following this link: [https://discord.com/api/oauth2/authorize?client_id=893178480303407135\&permissions=268435456\&scope=applications.commands%20bot](https://discord.com/api/oauth2/authorize?client_id=893178480303407135\&permissions=268435456\&scope=applications.commands%20bot)

## 3. Assign the Lunar Commander Role

Upon adding the Lunar Assistant to your server, the Lunar Assistant slash commands will be registered with your server, and the `Lunar Commander` role will be created. Only those with the `Lunar Commander` role will be able to run Lunar Assistant configuration commands, so assign the `Lunar Commander` role to everyone that you want to be able to configure Lunar Assistant.

## 4. Create Your Hierarchy of Roles! 

Create the roles that you will use to manage the server. Place the "Lunar Assistant" role above any roles the bot is assigning. This is necessary for Lunar Assistant to assign roles properly.

## 5. Configure the Lunar Assistant 

Configure the Lunar Assistant to your liking via the relevant `/lunar-configure` commands. Learn more about assigning roles based on wallet holdings in the Token Permissioned Roles page:

{% content-ref url="token-permissioned-roles.md" %}
[token-permissioned-roles.md](token-permissioned-roles.md)
{% endcontent-ref %}

## 6. Create Private Channels

Create private channels and give select roles access. Then, users of certain token holdings will be granted access to these private channels via roles assigned by Lunar Assistant.

## 7. It's Up To Your Imagination!

You now have a basic configuration setup for Lunar Assistant. What you do with it is up to your imagination!
