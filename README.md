# CasparCG
## Installation

1. Clone\pull project files into the necessary directory.
2. Configure your web server's document / web root to be the project's `public` directory.
3. Install necessary php dependencies: `php composer.phar install` or `composer install (if composer already installed on your machine)`.
4. Configure directories access rights.
    - directories within the `storage` and the `bootstrap/cache` directories should be writable by your web server.
    - create a symbolic link at `public/storage` which points to the `storage/app/public` directory.
5. Configure your database, create user and db for this project `optional`.
6. Create `.env` with all necessary environment variables.
    - use `.env.example` for reference to fill all the settings including db, mail, memcached, etc.
    - set your application key to a random string `php artisan key:generate`.
7. Run all db migrations `php artisan migrate`.
8. Try to open your application in the web browser ^^
