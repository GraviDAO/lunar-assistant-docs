# Discord Bot Setup Quick Start

## 1. Create a Discord Server

You can use an existing server for which you are an admin, or use the following guide to create a new server: [https://support.discord.com/hc/en-us/articles/206143407](https://support.discord.com/hc/en-us/articles/206143407)

## 2. Add Lunar Assistant to your Discord Server

You can add Lunar Assistant to your Discord Server by following this link: [https://discord.com/api/oauth2/authorize?client\_id=1007464384492212254\&permissions=268435456\&scope=applications.commands%20bot](https://discord.com/api/oauth2/authorize?client\_id=1007464384492212254\&permissions=268435456\&scope=applications.commands%20bot)

## 3. Assign a role to the admin commands

Upon adding the Lunar Assistant to your server, the Lunar Assistant slash commands will be registered with your server. By default, Lunar Assistant configuration and poll commands are restricted, so assign these commands to everyone that you want to be able to configure Lunar Assistant.

Here is how we did it: \
1- We created an admin role for Lunar Assistant called Lunar Commander. Feel free to use any name you prefer for the admin role.\
2- We assigned all our admin users to Lunar Commander. \
3- Finally we allowed the configure and poll commands to Lunar Commander as you can see in the screenshots below:

![](<../../.gitbook/assets/image (3).png>)

![](<../../.gitbook/assets/image (3) (1).png>)

&#x20;![](<../../.gitbook/assets/image (1) (1).png>)

## 4. Create Your Hierarchy of Roles!&#x20;

Create the roles that you will use to manage the server. Place the "Lunar Assistant" role above any roles the bot is assigning. This is necessary for Lunar Assistant to assign roles properly.

## 5. Configure the Lunar Assistant&#x20;

Configure the Lunar Assistant to your liking via the relevant `/lunar-configure` commands. Learn more about assigning roles based on wallet holdings in the Token Permissioned Roles page:

{% content-ref url="token-permissioned-roles.md" %}
[token-permissioned-roles.md](token-permissioned-roles.md)
{% endcontent-ref %}

## 6. Create Private Channels

Create private channels and give select roles access. Then, users of certain token holdings will be granted access to these private channels via roles assigned by Lunar Assistant.

## 7. It's Up To Your Imagination!

You now have a basic configuration setup for Lunar Assistant. What you do with it is up to your imagination!
