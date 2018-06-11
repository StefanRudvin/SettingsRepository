# common-intellij-settings

These are our shared intellij settings.

## Adding to your IDE

Go to **Intellij IDEA > Preferences > Tools > Settings Repository** and add `git@git.hubteam.com:HubSpot/common-intellij-settings.git` as a read-only source:

![](https://git.hubteam.com/storage/user/589/files/58259afc-6d7f-11e8-844e-10346e02afe2)

## Building a settings jar

You can build a new settings jar by running the following from the repo root.
```shell
jar cf settings-$(date +'%Y-%m-%d').jar *
```
