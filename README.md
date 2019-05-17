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
## Deploy
Before deploy your website remember these steps, i've tested it on Ubuntu 18.04
You have a **docker-compose-prod.yml**, run this command
```
docker-compose -f docker-compose-prod.yml up -d
```
### Problem with uploads
There is a problem with file uploads, i've find this workaround for the moment
```
sudo find wp-content/ -type d -exec chmod 777 {} +
```




