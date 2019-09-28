Toy App
=========

This is simple Ruby app using the Rails framework, deployed on heroku.

## Routes
* [Home](https://toy-app-rails-tutorial-michael.herokuapp.com/)
* [View users]( https://toy-app-rails-tutorial-michael.herokuapp.com/users)
* [Create user]( https://toy-app-rails-tutorial-michael.herokuapp.com/users/new)
* [View microposts]( https://toy-app-rails-tutorial-michael.herokuapp.com/mircroposts)
* [Create mircropost]( https://toy-app-rails-tutorial-michael.herokuapp.com/microposts/new)

## Running Locally
------------------

Make sure you have [Ruby](https://www.ruby-lang.org), [Bundler](bundler.io) and the [Heroku Toolbelt](https://toolbelt.heroku.com) installed.

```sh
git clone https://github.com/SG24/toy_app.git # or clone your own fork
cd toy_app
bundle install --without production # uses sqlite3 in development, but needs postgresql while deploying on heroku
rails server
```

Your app should now be running on [localhost:3000](http://localhost:3000/).

## Deploying to Heroku

```sh
heroku create
git push heroku master
heroku run rake db:migrate
heroku open
```

Alternatively, you can deploy your own copy of the app using the web-based flow:

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

## Documentation

For more information about using Ruby on Heroku, see these Dev Center articles:

- [Ruby on Heroku](https://devcenter.heroku.com/categories/ruby)
- [Getting Started with Ruby on Heroku](https://devcenter.heroku.com/articles/getting-started-with-ruby)
- [Heroku Ruby Support](https://devcenter.heroku.com/articles/ruby-support)
