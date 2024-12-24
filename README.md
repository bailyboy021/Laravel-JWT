# Laravel-JWT

A simple implementation of JWT authentication in Laravel using the tymon/jwt-auth package.

## Installation

1.  Clone the repository:

    ```bash
    git clone https://github.com/bailyboy021/Laravel-JWT.git
    ```

2.  Navigate to the project directory:

    ```bash
    cd Laravel-JWT
    ```

3.  Install Composer dependencies:

    ```bash
    composer install
    ```

4.  Copy the `.env.example` file to `.env` and configure your environment variables (especially database credentials):

    ```bash
    cp .env.example .env
    ```

    Buka file `.env` dan sesuaikan pengaturan database Anda. Contoh:

    ```
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=laravel_jwt
    DB_USERNAME=root
    DB_PASSWORD=
    ```

5. Generate JWT secret key:

    ```bash
    php artisan jwt:secret
    ```
    This command will generate a JWT secret key and add it to your `.env` file as `JWT_SECRET`.

6.  Generate application key:

    ```bash
    php artisan key:generate
    ```

7.  Run database migrations:

    ```bash
    php artisan migrate
    ```

8.  Serve the application:

    ```bash
    php artisan serve
    ```

    This will start the development server at `http://127.0.0.1:8000`.
