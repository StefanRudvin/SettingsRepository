# intellij-settings

These are our shared intellij settings.

## Adding to your IDE

Go to **Intellij IDEA > Preferences > Tools > Settings Repository** and add `git@git.hubteam.com:HubSpot/intellij-settings.git` as a read-only source:

![](https://git.hubteam.com/storage/user/589/files/7633b8d6-4871-11e8-9c24-17a6afdc2e7d)

## Building a settings jar

You can build a new settings jar by running
```shell
jar cf settings-$(date +'%Y-%m-%d').jar *
```
