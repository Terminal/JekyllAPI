---
date: 2019-04-17
title: How to create a Discord webhook to send GitHub repository updates to your Discord channel
description: Learn how to create a Discord webhook to send GitHub repository updates to keep up to date with what your development team is doing on GitHub.
---

## How to install
1. Create or find an existing channel where your notifications will appear
2. Click on the `Edit Channel` button next to the channel name  
   ![Click Settings](/assets/img/howto/20190417-add-github-webhook/editchannel.png)
3. Within the `Webhooks` tab, click on the `Create Webhook` button  
   ![Create Webhook](/assets/img/howto/20190417-add-github-webhook/createwebhook.png)
4. Click the `Copy` button next to the URL that has been generated by Discord
  - You may change the `Name` and `Webhook Icon`, but this will have no effect
    as the GitHub icon and name will override your settings.  
   ![Copy Webhook](/assets/img/howto/20190417-add-github-webhook/copywebhook.png)
5. Enter the settings tab of the repository you wish to obtain push notifications from  
   ![Click Settings](/assets/img/howto/20190417-add-github-webhook/clicksettings.png)
6. In the `Webhooks` tab, click the `Add webhook` button on the right hand side of the screen.  
   ![Add Webhook](/assets/img/howto/20190417-add-github-webhook/addwebhook.png)
7. Paste the link you copied earlier, and at the end of the URL, add `/github`
8. Change the `Content type` to `application/json`  
   ![Appending `/github` to the URL](/assets/img/howto/20190417-add-github-webhook/editpayload.gif)
9. Select the level of events you wish to obtain
10. Click the `Add webhook` button

## Conclusion
After following all steps, future GitHub pushes, and additional events that you may have selected
will have notifications appear in the Discord channel you selected.

If there are no notifications pushed when you commit,
try joining [our Discord server]({{site.data.strings.discord}}) for one on one help.