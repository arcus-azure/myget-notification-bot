# MyGet Bot for GitHub Pull Requests/Issues
A bot to post comments on GitHub pull requests when a new NuGet package is pushed to MyGet.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Farcus-azure%2Fmyget-notification-bot%2Fmaster%2Fsrc%2Fazuredeploy.json" target="_blank">
    <img src="https://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Farcus-azure%2Fmyget-notification-bot%2Fmaster%2Fsrc%2Fazuredeploy.json" target="_blank">
    <img src="./media/logos/armviz.png"/>
</a>

# Prerequisites
- An Azure subscription
- Access to a MyGet account
- GitHub user that will be used to post comments
- Push NuGet versions in format of `PR-{pr-id}`, but you can also tweak the template to use your pattern

# Deployment
1. Deploy the ARM template in `src` or use the "Deploy to Azure" button
2. Create a new webhook registration on your MyGet feed for 'Package Added' events
3. All set!

# License Information
This is licensed under The MIT License (MIT). Which means that you can use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the web application. But you always need to state that Tom Kerkhove is the original author of this web application.