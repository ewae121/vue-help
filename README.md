# Vue 2 help

Memo on what was interesting things about VueJs

## Install a clean version on Ubuntu 20.04 with vue-cli command

* Ensure that nodejs package is not installed

```
sudo apt remove nodejs
```

In a new bash, **__npm__** command should not be available anymore.


* Install NVM:

```
curl -sL https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh -o install_nvm.sh
bash install_nvm.sh
source ~/.profile
```

Install the right version from NVM:

```
nvm install 14.5
nvm use 14.5.0
nvm alias default 14.5.0
nvm alias default node
```

and start a new bash

## Project setup

```
npm install
```

Install @vue/cli 4.5.9
-----------

* Ensure that vue-cli package 2.9.6 is not installed. Otherwise vuetify will not be installable.

```
npm remove vue-cli
npm remove -g vue-cli
```

In a new bash, **__vue__** command should not be available.

```
npm install -g @vue/cli
```

and start a new bash

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
