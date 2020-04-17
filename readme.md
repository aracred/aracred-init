# aracred-init

A CLI for setting up an Aracred instance

## Prerequisites

    * An [Ethereum Address](https://metamask.io) with some [ETH](https://www.sendwyre.com)
    * An [Aragon DAO](http://mainnet.aragon.org/#/create) (you need at lest 0.1 ETH to deploy your own DAO)
    * A [GitHub](https://GitHub.com) Account
    * A [Infura](https://infura.io)

## Setup Aracred Instance

Create a Local version of Aracred configured to your DAO

```sh
npx aracred-init
```

This will create `./aracred-template` folder in your working directory

## Prepare Your repo

1. create a new repository in your organisation and name it Aracred
2. in the settings section of your repo, navigate to `Actions` and select `Enable local and third party Actions for this repository`
3. also in settings, navigate to `Secrets` and add your infura key as `INFURA_KEY`, and your Ethereum private key as `PRIVATE_KEY`.

## Launch Aracred

To Launch Aracred you simply need to push your local version to your new repo. In `./aracred-template`

```sh
git init
git remote add origin https://github.com/pythonpete32/Aracred.git
git push -u origin master
```
