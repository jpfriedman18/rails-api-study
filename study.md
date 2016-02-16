# Rails as an API Study

Use your favorite search engine and the provided readings to research and answer
the following questions (no prior knowledge is expected).

In your answers, be sure to cite any relevant sources you consulted in your
search. We ask you to write answers in your own words in order to see how you
process what you've read. Please do not answer with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

Please note:

-   Many of the readings will mention the "view" layer. We won't be covering the
    view layer in this program.
-   For now, we'll use the `rails-api` gem to create rails applications.
    `rails-api` is set to become part of Rails 5. We will never type `rails
    new`, instead preferring `rails-api new`.

## Required Readings

-   [Starting Ruby on Rails: What I Wish I Knew | BetterExplained](http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/)
-   [Intermediate Rails: Understanding Models, Views and Controllers | BetterExplained](http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/)
-   [Getting Started with Rails — Ruby on Rails Guides](http://guides.rubyonrails.org/getting_started.html)
-   [The Rails Command Line — Ruby on Rails Guides](http://guides.rubyonrails.org/command_line.html)
-   [Rails Routing from the Outside In — Ruby on Rails Guides](http://guides.rubyonrails.org/routing.html)
-   [Action Controller Overview — Ruby on Rails Guides](http://guides.rubyonrails.org/action_controller_overview.html)

## Define Model Responsiblities

In your own words, define what the responsibilities of the model layer are in
Rails.

```md
The model takes commands from the controller and then executes them by finding
and retrieving information from the database on the back-end.
```

## Define Controller Responsiblities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md
The controller facilitates interactions between the browser on the front-end,
and components on the back-end. On the client side, it takes requests for information
or data submissions, then passes them along to components on the back-end, either
the model (in order to get information from the database) or the view (in order
to render what the user is supposed to see)
```

## Define Router Responsiblities

In your own words, define what the router does in Rails.

```md
The router takes a URL from the browser, and uses it to determine which controller
to use to access the back-end, and then tell that controller what data or actions
are required to satify the user's request
```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md
The browser passes a request to a web server, which uses the router to determine
which controller to use. The controller then determines from the request what
actions or information are needed, and sends a request to the model, which then
returns the correct item from the database. The controller receives this information
and passes it to the view, which generates the necessary code to create what the
user will see and how they will see it, then sends that information back to the
controller, which sends it back to the browser via the web server for use by
the user.
```
