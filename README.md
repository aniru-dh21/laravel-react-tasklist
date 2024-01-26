# Using React.js with Laravel to Build a Draggable Tasklist App

**Tasklist single-page, full-stack app built with Laravel and React.js (with Vite.js). For the drag & drop functionality `react-beautiful-dnd` is used.**

As a backend framework, Laravel actually offers a tool to help you do this, called [Inertia](https://laravel.com/docs/10.x/frontend#inertia). Here's what the docs say about it:

> It bridges the gap between your Laravel application and your modern Vue or React frontend, allowing you to build full-fledged, modern frontends using Vue or React while leveraging Laravel routes and controllers for routing, data hydration and authentication - all within a single code repository.

## Pre-requisites

- PHP >= 8.1 (run `php -v` to check the version)
- Composer (run `composer` to check that it exists)
- MySQL >= 5.7 (run `mysql --version` to check if it exists, or follow the [docs](https://dev.mysql.com/doc/mysql-windows-excerpt/5.7/en/windows-testing.html))
- Node.js >= 18 (run `node -v` to check the version)

## Installation:

1. Clone the repository, or download the zip file and extract it.
```shell
git clone git@github.com:boolfalse/laravel-react-tasklist.git && cd laravel-react-tasklist/
```
2. Copy the `.env.example` file to `.env`:
```shell
cp .env.example .env
```
3. Install the dependencies
```shell
composer install
```
4. Generate the application key.
```shell
php artisan key:generate
```
5. Create a MySQL database and set the database credentials in the `.env` file:
```shell
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE="<database_name>"
DB_USERNAME="<username>"
DB_PASSWORD="<password>"
```
6. **_[Optional]_** To change the default seed data (projects, tasks counts) update `config/project.php` file, and optimze caches as mentioned below
7. Refresh the application cache.
```shell
php artisan optimize
```
8. Run the migrations and seed the database.
```shell
php artisan migrate:fresh --seed
```
9. Install the NPM dependencies.
```shell
npm install
```
10. Build the assets
```shell
npm run build
```
11. **_[Optional]_** For development, run below command to watch the assets for changes.
```shell
npm run dev
```
12. Start the development server using below command or configure a virtual host.
```shell
php artisan serve
```
13. Open the application in a browser at [http://127.0.0.1:8000](http://127.0.0.1:8000/)

## Resources

[Postman Collection](https://documenter.getpostman.com/view/1747137/2s9YsJArg7)
