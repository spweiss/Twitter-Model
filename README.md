# Twitter Model

This is a web model for Twitter developed in Ruby on Rails according to MVC and
REST architectural models. It incorporates a full suite of features, including:

* Users (with unidirectional following, administrator privileges, and user indices)
* Microposts (with news feeds, pagination, and image attachment)
* Sign-up and log-in (with email verification, password reset, and SSL encryption)

The application is deployed using Heroku to handle database storage (for the
user, micropost, and following models) and for (relatively) scalable server use.

## View

View the deployed Twitter Model [here](http://www.twitter-model.herokuapp.com/).

## Getting started

To get started with the app, clone the repo and then install the needed gems:

```
$ bundle install --without production
```

Next, migrate the database:

```
$ rails db:migrate
```

If you would like to populate the model with sample users, run:

```
$ rails db:seed
```

Finally, run the test suite to verify that everything is working correctly:

```
$ rails test
```

If the test suite passes, you'll be ready to run the app in a local server
(depending on your browser and OS of choice, you may need to set the IP to
0.0.0.0 rather than the default localhost if rails protests):

```
$ rails server
```
```
$ rails server -b 0.0.0.0
```

## Ruby on Rails Tutorial

This is based on [Michael Hartl](http://www.michaelhartl.com/)'s excellent text
on web development in rails: [*Ruby on Rails Tutorial: Learn Web Development
with Rails*](http://www.railstutorial.org/).

## License

All source code in the [Ruby on Rails Tutorial](http://railstutorial.org/)
is available jointly under the MIT License and the Beerware License. See
[LICENSE.md](LICENSE.md) for details.
