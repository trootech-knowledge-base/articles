---
layout: post
title: Laravel Installation Guide
subtitle: Step-by-step guide to installing Laravel
categories: Laravel
tags: [installation, Laravel, guide]
top: 1
new: 1
iVBORw0KGgoAAAANSUhEUgAABkAAAASwCAYAAACjAYaXAAAACXBIWXMAAB2HAAAdhwGP5fFlAAAFGmlUWHRYTUw6Y29tLmFkb2JlLnhtcAAAAAAAPD94cGFja2V0IGJlZ2luPSfvu78nIGlkPSdXNU0wTXBDZWhpSHpyZVN6TlRjemtjOWQnPz4KPHg6eG1wbWV0YSB4
sidebar: []
---

This guide walks you through installing [Laravel][1] step by step.

## Laravel Installation Guide

*Note: This guide assumes you have basic knowledge of PHP and Composer.*

## Prerequisites

Before installing Laravel, ensure you have the following:

- **PHP (>= 8.0)** – Laravel requires PHP 8.0 or higher.
- **Composer** – Laravel uses Composer to manage dependencies.
- **Web Server** – Apache or Nginx.
- **Database** – MySQL, PostgreSQL, SQLite, or SQL Server.

## Installing Laravel

### Using Composer

Run the following command in your terminal:

```sh
composer create-project --prefer-dist laravel/laravel my-laravel-app
```

This command installs Laravel in a new directory called `my-laravel-app`.

### Verifying Installation

Navigate into your project folder:

```sh
cd my-laravel-app
```

Start the local development server:

```sh
php artisan serve
```

Open `http://127.0.0.1:8000` in your browser. If you see the Laravel welcome page, your installation is successful.

## Configuring Environment

Laravel uses an `.env` file for environment configuration. Copy the example file:

```sh
cp .env.example .env
```

Then generate an application key:

```sh
php artisan key:generate
```

## Database Configuration

Update your `.env` file with database details:

```ini
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=root
DB_PASSWORD=
```

Run migrations to set up the database:

```sh
php artisan migrate
```

## Running Your Laravel Application

Use the built-in PHP server:

```sh
php artisan serve
```

Or configure a virtual host in Apache/Nginx for better performance.

## Conclusion

You have successfully installed Laravel! Explore the framework and build amazing applications.

For more details, visit the official [Laravel documentation][2].

---

## Additional Resources

- [Laravel Documentation][2]
- [Composer Documentation][3]
- [PHP Official Site][4]

[1]: https://laravel.com/
[2]: https://laravel.com/docs
[3]: https://getcomposer.org/doc/
[4]: https://www.php.net/
