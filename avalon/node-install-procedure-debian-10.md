# Avalon  install procedure for debian 10:
```bash
## Make sure system is up to date
sudo apt-get update
sudo apt-get upgrade
## Install some common tools
sudo apt-get install git wget tmux htop jq
## Clone avalon
git clone https://github.com/dtube/avalon.git
cd avalon/
```

```bash
## Install node+npm
sudo apt-get install nodejs npm
```

```bash
node -v
## If not on node v10, install nvm
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
nvm install v10
nvm use v10
```

```bash
## MongoDB
wget -qO - https://www.mongodb.org/static/pgp/server-4.2.asc | sudo apt-key add -
echo "deb http://repo.mongodb.org/apt/debian buster/mongodb-org/4.2 main" | sudo tee /etc/apt/sources.list.d/mongodb-org-4.2.list
sudo apt-get update
sudo apt-get install -y mongodb-org
```

```bash
## NPM packages
npm install
```

```bash
## Download genesis.zip
mkdir genesis && cd genesis
wget https://backup.d.tube/genesis.zip
cd ..
```

## Environment variables
See the `scripts/start.sh` file for a list of important environment variables
```bash
#!/bin/bash

# Ports configuration
#export HTTP_PORT=3001
#export P2P_PORT=6001

# MongoDB configuration
#export DB_NAME=avalon
#export DB_URL=mongodb://localhost:27017

# Peering configuration
#export OFFLINE=1
#export NO_DISCOVERY=1
#export DISCOVERY_EXCLUDE=dtube

# Enable more modules
#export NOTIFICATIONS=1
#export RANKINGS=1

# Cache warmup option
export WARMUP_ACCOUNTS=100000
export WARMUP_CONTENTS=0

# Warn when a transactions takes more than X ms
export WARN_SLOW_VALID=5
export WARN_SLOW_EXEC=5

# trace / perf / econ / cons / debug / info / warn
export LOG_LEVEL=debug

# groups blocks during replay output to lower screen spam
export REPLAY_OUTPUT=1

# default peers to connect with on startup
export PEERS=ws://34.65.228.228:6001
export MAX_PEERS=20

# your user and keys (only useful for active node owners)
export NODE_OWNER=<username>
export NODE_OWNER_PUB=<a public key>
export NODE_OWNER_PRIV=<a private key>

node --stack-size=65500 src/main
```

Then start with `./scripts/start.sh`
