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


Nice example
-------------

[Creative Tim Dashboard example](https://demos.creative-tim.com/vuetify-material-dashboard/#/)


Cool Libs
-----------

### Vue Router

Manage routing in application (Official)

Installation

```
vue add router
```

Official documentation

[Vue Router documentation](https://router.vuejs.org/)


### Vuex

Store to share data between components (Official)

Installation

```
vue add vuex
```

Official documentation

[Vuex documentation](https://vuex.vuejs.org/)


### Vue-i18n

Locales management (Official)

Installation

```
vue add i18n
```

Official documentation

[Vue i18n documentation](https://kazupon.github.io/vue-i18n/introduction.html#sponsors)


### Vuetify

Vuetify is a complete UI framework built on top of Vue.js. The goal of the project is to provide developers with the tools they need to build rich and engaging user experiences.


Installation

```
vue add vuetify
```

Official documentation

[Vuetify documentation](https://vuetifyjs.com/en/introduction/why-vuetify/)


### ChartJs

Components to make great charts

Installation

```
npm install vue-chartjs
```

Official documentation

[ChartJs documentation](https://www.chartjs.org/)
[ChartJs sample](https://www.chartjs.org/samples/latest/)


### Vue Grid layout

Help to make complex grid layout with drag and drop, resize...

Installation

```
npm install vue-grid-layout --save
```

Official documentation

[Vue Grid Layout documentation](https://jbaysolutions.github.io/vue-grid-layout/)
