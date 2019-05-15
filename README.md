# wdwtb
Wordpress Docker Webpack Timber Bootstrap

## Before starting
Make sure you have insalled these dependencies

- [Docker](https://docs.docker.com/).
- [NodeJs](https://nodejs.org/it/download/).
- [NPM](https://www.npmjs.com/get-npm).
- [Composer](https://getcomposer.org/download/).

## Install dependencies
```
cd theme
npm install
composer install
```
## Develop
Start docker
```
docker-compose up
```
Start webpack watcher
```
npm run watch
```
## Build
```
npm run production
```
