# Install-Microsoft-Onedrive-on-Ubuntu-20.04

This article is to record and share my installation of Onedrive.

The app to download is of course from : https://github.com/abraunegg/onedrive/blob/master/docs/INSTALL.md

I am using PPA, so : https://launchpad.net/~yann1ck/+archive/ubuntu/onedrive

```
$ sudo add-apt-repository ppa:yann1ck/onedrive
$ sudo apt-get update
$ onedrive
Configuring Global Azure AD Endpoints
Authorize this app visiting:

https://login.microsoftonline.com/common/oauth2/v2.0/authorize?client_id=d50ca740-c83f-4d1b-b616-12c519384f0c&scope=Files.ReadWrite%20Files.ReadWrite.all%20Sites.Read.All%20Sites.ReadWrite.All%20offline_access&response_type=code&redirect_uri=https://login.microsoftonline.com/common/oauth2/nativeclient
```
You will be asked if you will let this app access your info.  Click "Yes" and what follows is a blank page.  Copy the url and paste it in the terminal and you should see this response:

```
Application has been successfully authorised, however no additional command switches were provided.

Please use --help for further assistance in regards to running this application.
```

To start using Onedrive, 

```
$ onedrive --synchronize
```

It will start to download your Onedrive files and folders into your local machines under the directory home/OneDrive





