Symfony + Chaplin + Backbone TodoMVC
====================================

This a skeleton app for a [Symfony](http://symfony.com) version of [TodoMVC](http://todomvc.com/).
It uses [DunglasTodoMVCBundle](http://dunglas.fr/2013/02/symfony-2-todomvc-backbone-chaplin/).

Demo
----

Try it online: http://symfony-todomvc.dunglas.fr/

Install
-------

Install the [Composer](http://getcomposer.org/) dependency  manager if you don't already have it.
Of course, you need PHP, a web server running PHP (tested with Apache) and a database (works fine with SQLite and MySQL).

Go to the application directory and install dependencies:

    composer install

Copy `app/config/parameters.yml-dist` to `app/config/parameters.yml` and edit it to match your local configuration.

Install assets:

    php app/console assets:install web

Dump assets if you want to use the app in prod mode:

    php app/console assetic:dump --env=prod --no-debug

Create database schema:

    php app/console doctrine:schema:create

Make `web` the document root of your web server.

Done! Open *http://localhost/app_dev.php* in your browser and try this Symfony implementation of TodoMVC.

Security
--------

TodoMVC is unsecure by design. Everyone can do everything.
If you create a real world Symfony + Backbone.js app be sure to add an authentification system and a CSRF protection layer.

Credits
-------

This bundle has been created by [Kévin Dunglas](http://dunglas.fr).
The CoffeeScript code is largely inspired of the [Brunch + Chaplin TodoMVC implementation](https://github.com/addyosmani/todomvc/tree/gh-pages/labs/dependency-examples/chaplin-brunch) of [Paul Millr](http://paulmillr.com/).
