# common-intellij-settings

These are our shared intellij settings. Using the fork distribution method provided below, you can merge in changes as we update the base settings.

## Adding to your IDE

### Fork this repo to your personal GitHub org
Click fork:
![fork](https://git.hubteam.com/storage/user/589/files/ed4d40a2-73c0-11e8-9d6e-61dec405fd17)

### Click `Settings Repository...`

![](https://git.hubteam.com/storage/user/589/files/59f4b5f0-73c1-11e8-9ccc-2ec5b0b0cdc1)

**or**

![](https://git.hubteam.com/storage/user/589/files/28c5c18a-73c2-11e8-8b89-6d2d1bc11a9f)

### Add your fork

Get your repository URL:

![](https://git.hubteam.com/storage/user/589/files/52882e72-73c2-11e8-8c83-87a1bd4dd963)

Add it and click `merge`:

![](https://git.hubteam.com/storage/user/589/files/64b06e16-73c2-11e8-9b33-19af6a094db8)

#### Troubleshooting
If this stage fails with an `Auth fail` message, simply clone your settings repo and point IntelliJ to the local directory.

### Migrating to this set up

The above steps should work for you. One gotcha is that our Java style module has been renamed to `HubSpotDefault` from `Default (1)`. You can migrate your settings before merging things in by copying [this PR](https://git.hubteam.com/HubSpot/intellij-settings/pull/4).

## Updating your fork

Updating your fork is easy, if done correctly.

### Sync your current settings and quit IntelliJ

Go to **VCS > Sync Settings > Overwrite Remote**

![](https://git.hubteam.com/storage/user/589/files/bef8478e-73c4-11e8-96de-842b31c820ff)

### Clone your fork and cd into it

### Get upstream changes on your fork

### Add remote
```bash
git remote add upstream git@git.hubteam.com:HubSpot/intellij-settings.git
```

#### Follow [the GitHub guide](https://help.github.com/articles/syncing-a-fork/)

#### Push
```bash
git push origin master
```

### Pull in the changes to IntelliJ

Open IntelliJ and do **VCS > Sync Settings > Overwrite Local**

![](https://git.hubteam.com/storage/user/589/files/91e84270-73c5-11e8-8d0c-794190ed7bf4)

## Building a settings jar

You can build a new settings jar by running the following from the repo root.
```shell
jar cf settings-$(date +'%Y-%m-%d').jar *
```
