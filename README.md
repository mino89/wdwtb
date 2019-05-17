# wdwtb
Wordpress Docker Webpack Timber Bootstrap

## Before starting
Make sure you have insalled these dependencies

- [Docker](https://docs.docker.com/).
- [NodeJs](https://nodejs.org/it/download/).
- [NPM](https://www.npmjs.com/get-npm).
- [Composer](https://getcomposer.org/download/).

### Set Up environment variables
Export these three variables
```
export DB_ROOT_PWD="yourpassword"
export DB_PWD="yourpassword"
export DB_USer="youruser"
```

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
