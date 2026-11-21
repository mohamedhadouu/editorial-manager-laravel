# Editorial Manager for a Scientific Journal (Laravel)

A web platform to manage the publication workflow of a scientific journal: **authors submit articles, editors and reviewers handle the review, and accepted articles are published** on a public page.

![PHP](https://img.shields.io/badge/PHP-Laravel-red) ![CSS](https://img.shields.io/badge/CSS-Tailwind-38bdf8) ![Build](https://img.shields.io/badge/Build-Vite-purple)

## Features

- **Four roles** with separate authentication: Author, Editor, Reviewer, Admin
- **Author space**: registration, email verification code, login, password reset, article submission
- **Editor and Reviewer spaces**: manage and review submitted articles
- **Admin dashboard**: manage the platform
- **Public pages**: list of accepted articles, article search, contact page

## Tech stack

PHP · Laravel · MySQL · Blade · Tailwind CSS · Vite

## Project structure

| Folder | Content |
|---|---|
| `app/Http/Controllers/` | Controllers for each role (Author, Editor, Reviewer, admin, article) |
| `database/migrations/` | Tables: users, authors, editors, reviewers, articles |
| `resources/views/` | Blade templates for each dashboard |
| `routes/web.php` | Routes grouped by role with dedicated guards |

## How to run

```bash
git clone https://github.com/mohamedhadouu/editorial-manager-laravel.git
cd editorial-manager-laravel
composer install
npm install
cp .env.example .env
php artisan key:generate
```

Set your database credentials in `.env`, then:

```bash
php artisan migrate
npm run dev
php artisan serve
```

Open `http://localhost:8000` in your browser.

## Next steps

- Add screenshots of each dashboard to this README
- Add email notifications when an article changes status
- Write feature tests for the submission and review workflow

## Author

**Mohamed Hadou** · [LinkedIn](https://www.linkedin.com/in/mohamed-hadou/) · [GitHub](https://github.com/mohamedhadouu)
