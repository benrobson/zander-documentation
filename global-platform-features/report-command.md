# Report Command

This command is fairly simple. This command is a multi-platform command and feature since you can report users form 3 places \(in-game, Discord and the website \(/report\)\).

## Minecraft

{% hint style="info" %}
**Command:** /report  
**Usage:** /report \[username\] \[reason\]
{% endhint %}

If the user is to execute the command /report with it's correct usage 2 things happen.  
Users who are Server Operators or who have the `zander.reportnotify` permission node will have a message appear in chat.

![An example of what the command looks like operated in-game](../.gitbook/assets/image%20%283%29.png)

The second action is that it takes the same text and puts it in an embed message and sends it to the configured reports channel \(it's \#reports by default\).

![An example of what the command looks like operated in-game on Discord.](../.gitbook/assets/image%20%281%29.png)

## Website

![Example of filled out form on the /report page.](../.gitbook/assets/image%20%285%29.png)

On the website the user is to complete the report form. On submission 2 actions occur.  
The first action is that it takes the form and puts it in an embed message and sends it to the configured reports channel \(it's \#reports by default\).

![Example of the Discord embed report notification.](../.gitbook/assets/image.png)

The 2nd action is that a formatted template email is sent to the email address in the `notificationemail` configuration setting.

{% hint style="info" %}
The email feature will not work if the `mailsend` option is set to false.
{% endhint %}

![Example of the Discord embed report notification.](../.gitbook/assets/image%20%284%29.png)

