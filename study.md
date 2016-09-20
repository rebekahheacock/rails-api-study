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
-   We'll use our [rails-api-template](https://github.com/ga-wdi-boston/rails-api-template)
    repository as the basis for our rails applications.
    This template excludes the "view" layer.

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

The model layer interacts with the database and handles most of the
application logic.

```

## Define Controller Responsiblities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md

Controllers connect models and views. They help communicate between the models
(which interact with the database) and what the user of a web app ultimately
sees (the views). They also handle some basic application
functionality/features like authorization, redirects, and errors.

```

## Define Router Responsiblities

In your own words, define what the router does in Rails.

```md

The router parses a URL (books/create) and matches it with a controller action
(books#post).

```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md

The client makes a GET request to a URL. The web server uses routes to map
that request to an action in the controller. The dispatcher creates a
controller, calls that action, and passes any parameters. Depending on the
request, the controller gets or saves data from a model, then passes that data
to a view. The view generates the necessary HTML/client-side resources. The
controller passes that response body (HTML + other client-side resources),
plus metadata, back to the server. The server combines this information into
an HTTP response and sends it to the client.

```
