Heroku Symfony2 build pack
========================

This build pack is used to bundle Symfony2-based webapps and PHP-FPM+Nginx server for Heroku apps.

### Environment variables

This buildpack will add a few environment variables at compile time by parsing ``DATABASE_URL``:

- ``HEROKU_DATABASE_USER``
- ``HEROKU_DATABASE_PASSWORD``
- ``HEROKU_DATABASE_HOST``
- ``HEROKU_DATABASE_DB``
- ``HEROKU_DATABASE_PORT``

It also sets ``HEROKU_ASSETS_VERSION`` based on the date to have it during the slug compilation.

WARNING: READ ME!
-------------
**This build pack is strongly coupled & linked to our own app.**

A new build pack for Symfony2 will be rewritten soon by our team. It will be more efficient and less coupled to our app configuration.
You can find it here : https://github.com/Swop/heroku-buildpack-symfony2
