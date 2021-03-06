<p align="center">
<img src="https://viv.changewindows.org/img/logo_color.png" width="100px" height="auto">
</p>

<h3 align="center">ChangeWindows viv</h3>

<p align="center">
Changing viv one commit at a time
<br />
<br />
<a href="https://viv.changewindows.org">ChangeWindows viv</a>
&middot;
<a href="https://changewindows.org">ChangeWindows</a>
</p>

## About ChangeWindows
ChangeWindows does what Microsoft doesn't: document every change we can possibly find in Windows on any platform.

## Open source
This repository is a big shift for ChangeWindows from the previous 4 major versions. Not only is this the first time we're publishing the actual source of our website, we're also using for the first time a framework, in this case Laravel, to build our website. Not only because we're lazy, but also because it makes things a lot simpeler and cleaner.

## Using
To run ChangeWindows, you'll need the following:

* PHP 7.1.3 or higher, including extensions required by Laravel 5.7
* MySQL
* Composer
* NPM

### Setup
Clone this repository to any given directory and setup the `.env` file with all required parameters. An example of an `.env` file can be found in `.env.example`. Then execute the following commands.

```
composer install
npm install
php artisan migrate
php artisan db:seed
```

To run ChangeWindows, use the following command:

```
php artisan serve
```

This will launch a server at `127.0.0.1:8000`. Also run this NPM command.

```
npm run watch
```

This will compile various files, mostly SCSS and keep an eye out for changes.

### Login details
After migrating and seeding the database, there will be 3 accounts from the start.

| Name | Email | Role | Password |
| ---- | ----- | ---- | -------- |
| Yannick | yannick@changewindows.org | Admin | secret |
| Viv | viv@changewindows.org | Insider | secret |
| Tom | tom@changewindows.org | User | secret |

## Contributing
We are open to contributions to ChangeWindows. Do you have a feature that you really want to see but we are not spending any time on it ourselves? Feel free to open a pull request for it!

## Security Vulnerabilities
If you discover a security vulnerability within ChangeWindows, please contact us through private means. Most successful would probably be to contact us on [Twitter](https://twitter.com/changewindows).

## License
The ChangeWindows website is open-sourced software licensed under the [AGPL license](LICENSE). Note however that the content on our website isn't unless stated otherwise.
