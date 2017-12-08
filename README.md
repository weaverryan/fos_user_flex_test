# FOSUserBundle Symfony 4.0 Support Testing Project

See: https://github.com/FriendsOfSymfony/FOSUserBundle/pull/2639

1) Install composer deps:

```
composer install
```

2) Update the database schema (tweak `.env` first):

```
php bin/console doctrine:database:create
php bin/console doctrine:schema:create
```

3) Start the server:

```
php bin/console server:run
```

Now, surf around the site at `http://localhost:8000`! No
routes exist, except those from FOSUserBundle:

```
php bin/console debug:router
```

Use can use `/register` to create a user, then try logging in,
etc. Please help test everything - many features may not be fully
configured in the project. The config is in `config/packages/fos_user.yaml`.
