Buildpack: Null
=======================

This is a null [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks).

It does absolutely nothing.

Usage
-----

Example usage:

    $ ls
    .null

    $ heroku create --stack cedar --buildpack http://github.com/framp/buildpack-null.git

    $ git push heroku master
    ...
    -----> Heroku receiving push
    -----> Fetching custom buildpack
    -----> NullFramework app detected


Purpose
-------
This is useful only if there is something else doing something with your application.

I'm using it with dokku to store files server with nginx before proxying to apps
