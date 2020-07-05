# Sessions Controller Lab

## Objectives

We're going to build a Rails app that handles sessions with a
`SessionsController`. We won't have passwords—for now, we're going to ask the
user what to call them, and we'll just use that as their username.

## Introduction

Our app will have two pages:

1. A home page or root route.
   * If the user is not logged in, the page should show them a login link.
   * If the user is logged in, the page should say, "hi, #{name}", and provide a
   logout link.
2. A login page
   * Users can enter their name in a form and click 'login'. Thereafter, the app will
   refer to them by that name.
   * If the user does not enter a name, they are not logged in. Return them to the
   login page.

## Instructions

1. Create the sessions controller.

   **Note:** If you use the generators to generate your controllers, be sure to pass these
   flags to avoid generating unneeded files and routes: `rails generate controller Sessions new --no-helper --no-assets --no-test-framework --skip-routes --skip`. (For those who are curious, the `--skip` tag prevents the generator from conflicting with existing files.)

2. Write the `new`, `create`, and `destroy` methods.

3. Ensure that your tests pass!
