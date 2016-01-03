# Sessions Controller

## Objectives

We're going to build a Rails app that handles sessions with a `SessionsController`. We won't have passwords—for now, we're going to ask the user what to call them, and we'll just use that as their username.

## Introduction

Rails apps use `SessionsController`s to handle sessions. Today, we're going to implement this pattern.

Our app will have two pages:
  1. a home page. (`get '/'`)
    * if the user is not logged in, the page gives them a login link.
    * if the user is logged in, the page says, "hi, #{name}", and provides a logout link.
  2. a login page
    * users can enter their name and hit 'login'. Thereafter, the app will refer to them by that name.
    * if the user does not enter a name, they are not logged in. Return them to the login page.

## Instructions

You'll notice that there are a number of `SessionsController` specs failing because, principally, no `SessionsController` exists.

`rails generate controller Sessions new` to create a SessionsController with a `new` method. Controller method scaffolding is not generally that useful (you too can type `def new`!), but including `new` makes the generator create views, which we will also want.

Write `new`, `create`, and `destroy` methods to get the specs passing.

Now write feature tests for your views, write the views, and connect up your routes.