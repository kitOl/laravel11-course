# About Project

This code was created by [video](https://youtu.be/eUNWzJUvkCA)

## Extensions for VSCode

PHP Devsense
Laravel Blade formatter
Laravel Blade Snippets
Laravel Extra Intellisense
Laravel goto view
Auto Rename Tag
Highlight Matching Tag
Prettier - Code formatter
IntelliSense for CSS class names in HTML
Tailwind CSS IntelliSense

## How to

```bash
composer create-project laravel/laravel .
```

    this command create new projec in current place

```bash
npm install
```

this command install node app for css and js contents

```bash
npm run dev
```

this command run node app for css and js contents

Your css and js content you must place to resource folder in css and js folder.

For display this you need place in layout html in head section below title tag special tag:
`@vite(['resources/css/app.css', 'resources/js/app.js'])`

In results, Vite will be displaed this contents in browser.

For production release you need terminate npm run dev by `Ctrl+C` and enter new command:

```bash
npm run build
```

In result your browser will be show css and js from \*public folder.

Once your enter `npm run dev` browser will be show css and js from \*resource folder.

All is simple.

## Add Login in App

To add Login system in App you must install `breeze` package.
But before that you must save reserve copies for `app.css` and `web.php` files.
Next, enter new command:

```bash
composer require laravel/breeze --dev
```

and next:

```bash
php artisan breeze:install
```

and choose `Breeze stack` as `blade` and next `no` , ``.

Next, you must change `.env`:

```code
MAIL_MAILER=log
MAIL_HOST=127.0.0.1
MAIL_PORT=1025
```

and clear `storage/logs/laravel.log`.

Next, goto main page website and choose `Register`.
Input name, password and etc.
Will be sending email to confirm register.
This message saved in logs in `storage/logs/laravel.log`
