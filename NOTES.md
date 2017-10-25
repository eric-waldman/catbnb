Welcome to CatBnB
---------------

*CatBnB* is built using NodeJS and a bunch of awesome libraries. There are lots of moving parts and it can get overwhelming at times, but don't worry because all the concepts have been presented in Web 101 and Web 102 applications. After you're done you'll understand how each and everything works to create a modern web application.


The Home Controller
-----------------------

Our homepage's controller is `controllers/home.js`, where the following code listens for a request on the homepage URL

```
app.get(  '/', function( request, response ) {
  response.render( 'home' );
})
```

Here we listen to the path `/`, which is the homepage.  We call `render` on the response object with the `home` view as an argument so that Express generates the response HTML using the file `views/home.ejs`

The Home View
----------------------------

This is the template for our homepage.
It's a bit different than your standard HTML file.
For starters, EJS has its own comment tag
which you can see surrounding this comment.