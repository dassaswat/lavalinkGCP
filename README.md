# Lavalink Server || GCP Hosting

A solution for hosting lavalink server on google cloud platform using the compute engine. The server stays alive, as we will be using pm2.

## Installation on Ubuntu VM instance

First of all we need to get the update:

```bash
sudo apt update
```

Then we have to install node and npm and in order to do that we:

```bash
sudo apt install npm
```

Now we have to get nvm and install it!

```bash
curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash
```

Fetch the data with this command:

```bash
source ~/.profile
```

Now install it using:

```bash
nvm install node
```

## Java Installation

Installing Java Runtime environment & Java Development Kit and finally upgrading

```bash
sudo apt install openjdk-13-jre-headless
```

```bash
sudo apt install openjdk-13-jdk-headless
```

```bash
sudo apt upgrade
```

## Installation of Process Manager2(pm2) and setup

First we need to install pm2

```bash
npm i pm2 --g
```

Clone the following repository

```bash
git clone https://github.com/dassaswat/lavalinkGCP.git
```

Now we have to use the build command and we are done!

```bash
npm run build
```

## Available pm2 Commands

1. `bash pm2 start Lavalink`

2. `bash pm2 stop Lavalink`

3. `pm2 delete Lavalink`

4. `pm2 log Lavalink`

[Process Manager2 documentation](https://pm2.keymetrics.io/docs/usage/pm2-doc-single-page/)
