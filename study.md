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
The responsibility for the model layer is to chat to the backend. It talks to the database and also conducts backend logic (server side).
```

## Define Controller Responsiblities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md
The controller layer sorts out the incoming requests. It figures out where to send the requests and then does the same for the responses.
```

## Define Router Responsiblities

In your own words, define what the router does in Rails.

```md
The router waits for request at certain urls/or paths. Then the router will do a certain assigned function or feature.
```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md
GET
REQUEST
A client will make a GET request to a certain URL.
Hits the web server
then it hits the router
The router will then pass the request to the dispatcher
From the dispatcher it goes to the controller
the controller will the assign the request to the model.
The model will then conduct some backend logic
retrieve the item from the DB
RESPONCE
item gets passes from DB to Controller
controller then send item to WEB server
Web Server the send the item to the client.

```
