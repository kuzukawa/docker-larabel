# docker-larabel



This is docker-compose env to develop larabel on Docker using nginx, PHP and mysql.



## How to use

1. clone this repo

2. setup

   1. Type below to build docker-compose file.

      ```shell
      docker-compose up -d --build
      ```

   2. Install libraries for Larabel and copy .env.

      ```shell
      [host] docker-compose exec app bash
      [app]  composer install
      [app]  cp .env.example .env
      [app]  php artisan key:generate
      ```

   3. Check if database is connected.

      ```shell
      [app]  php artisan migrate
      ```

      

   