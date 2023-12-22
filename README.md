## Step to reproduce

execute the command:
- `docker-compose build`
- `docker-compose up -d`
- `docker-compose exec php bash`
- `composer install`
- `cp .env.example .env`
- `php artisan migrate`
- `php artisan queue:work`

open browser in localhost - job will be automatic dispatched (with transaction and without). Job without db transaction will be correct logged in db 
