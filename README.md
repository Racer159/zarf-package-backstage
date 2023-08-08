# zarf-package-backstage

An experimental Zarf package to play with [Spotify's Backstage](https://backstage.spotify.com/)

## create package

To create this package simply clone the repo and run:

```shell
$ zarf package create
```

Following the prompts as needed.

## deploy package

To deploy the created package onto an [initialized Kubernetes cluster](https://docs.zarf.dev/docs/zarf-tutorials/initializing-a-k8s-cluster) run:

```shell
$ zarf package deploy
```

And press `tab` to select the package you built earlier, following the prompts as needed.

## connect to backstage

To connect to backstage you will need to use a Chromium based browser and run:

```shell
$ zarf connect backstage --local-port 7007
```

> :warning: **Note:** This is the demo version of backstage which does not come configured for production - to add a demo component you can select "Create" from Home then "Register Existing Component" then enter a link to an entity file (i.e `https://github.com/backstage/backstage/blob/master/catalog-info.yaml`)

## remove package

To remove the package from your cluster when you are done run:

```shell
$ zarf package remove backstage
```
