## About Installation

This is a Laravel Project version 7.2
We will use laradock to run it locally. 
There is no need for learning Docker custom configurations for now

This is what you need: 
https://laradock.io/getting-started/#A1

The submodule is already, ready, so just 
```bash
cd api/laradock" and then 
```
hit "cp env-example .env" if not already exists.
After that type in your terminal 
```bash
docker-compose up -d nginx mysql
```
This will build the necessary containers, and allthough we use sqlite, you may wish to swith to mysql. 
To enter the container and run the artisan commands type:
```bash
docker-compose exec --user=laradock workspace bash
```
Then you will follow the typical laravel installation process. 
```bash
composer install
cp .env.example .env
php artisan key:generate
```

and change
DB_CONNECTION to sqlite
also delete the DB_DATABASE for more quick results
if you are planning to stick with sqlite. 

That's all!!!
Enjoy the api at your localhost!


## ABOUT FRONT END

# ybank

> ybank - frontend

## Build Setup

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev

# build for production and launch server
$ yarn build
$ yarn start

# generate static project
$ yarn generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).
