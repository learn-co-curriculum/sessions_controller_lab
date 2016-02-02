# Sessions Controller

## Objectives

We're going to build a Rails app that handles sessions with a `SessionsController`. We won't have passwords—for now, we're going to ask the user what to call them, and we'll just use that as their username.

## Introduction

Our app will have two pages:
  1. a home page or root route.
    * if the user is not logged in, the page should show them a login link.
    * if the user is logged in, the page should says, "hi, #{name}", and provide a logout link.
  2. a login page
    * users can enter their name in a form and click 'login'. Thereafter, the app will refer to them by that name.
    * if the user does not enter a name, they are not logged in. Return them to the login page.

## Instructions

1. Create the sessions controller.

*Note* If you use the generators to generate your controllers be sure to pass these flags to avoid generating unneeded files `rails generate controller Sessions new --no-helper --no-assets --no-controller-specs`.

2. Write the `new`, `create`, and `destroy` methods.

3. Write feature tests for your views that ensure the app functions as we described in the overview.

4. Create the views that make your tests pass!
