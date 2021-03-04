# LEMP環境

## usage

```
# GitHubからリポジトリをクローン
$ git clone https://github.com/AppRyu/docker_LEMP_environment.git
$ cd docker_LEMP_environment
$ docker-compose up -d --build
$ docker-compose exec app bash

# Laravelをインストール
[app] $ composer install
[app] $ cp .env.example .env
[app] $ php artisan key:generate
[app] $ php artisan migrate
[app] $ exit

$ docker-compose down
