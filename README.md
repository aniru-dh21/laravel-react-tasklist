# Using React.js with Laravel to Build a Draggable Tasklist App

**Tasklist single-page, full-stack app built with Laravel and React.js (with Vite.js). For the drag & drop functionality `react-beautiful-dnd` is used.**

As a backend framework, Laravel actually offers a tool to help you do this, called [Inertia](https://laravel.com/docs/10.x/frontend#inertia). Here's what the docs say about it:

> It bridges the gap between your Laravel application and your modern Vue or React frontend, allowing you to build full-fledged, modern frontends using Vue or React while leveraging Laravel routes and controllers for routing, data hydration and authentication - all within a single code repository.

## Pre-requisites

- PHP >= 8.1 (run `php -v` to check the version)
- Composer (run `composer` to check that it exists)
- MySQL >= 5.7 (run `mysql --version` to check if it exists, or follow the [docs](https://dev.mysql.com/doc/mysql-windows-excerpt/5.7/en/windows-testing.html))
- Node.js >= 18 (run `node -v` to check the version)
