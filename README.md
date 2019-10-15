# Talksuite PoT
## Demo dialogues & backend

This repo contains the code, template, dialogues and package to one click deploy a talksuite demo environment.

The button below will open Azure and prompt you with the infomation required to deploy this brige.

[![Deploy to Azure](https://azuredeploy.net/deploybutton.png)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fstrangecyan%2Ftalksuite-pot-demo%2Fmaster%2Ftemplates%2Ftemplate.json)

You will also need to deploy the appropriate dialogues to the talksuite organisation. To do so:
* Install the talksuite CLI by running `npm i @talksuite/talksuite-cli -g`.
* Log in to the CLI with your talksuite account by running `ts login`.
* Download or checkout this repo.
* Run the following command in the root folder `ts import-content ./dialogues/` and choose the organisation you want to use.

In talksuite your bot should be configured with:
* A constant called `cmsBaseUrl` with your  Strapi base url e.g. `https://your-deployment.azurewebsites.net`.
* The "Retail" project