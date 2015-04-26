What is this about?
===


We know WordPress is great for designing client sites and blogs, but so many designers don’t have the time to learn the WordPress Codex. **It’s huge. It’s intimidating. It’s confusing.**

That’s why I made this – a naked, **commented WordPress theme for designers who don’t want to deal with WordPress.** I’ve included all the basic units for a client site – *home page, about page, info page, blog page*, etc. I’ve included **comments on each and every piece of the WordPress puzzle**, so you can move things around intelligently, or remove them without worry.

For example, let’s look at the code underneath:

```
<?php wp_head(); 
// This fxn allows plugins, and WordPress itself, to insert themselves/scripts/css/files 
// (right here) into the head of your website. 
// Removing this fxn call will disable all kinds of plugins and WordPress default insertions. 
// Move it if you like, but I would keep it around.
?>
```
The whole thing is written in HTML5, where applicable and reliable, and comes with a responsive scaffold that you can use or throw away if you like.

Support for:
- Responsive styling
- Custom menus
- Custom sidebar and widgets
- Blog, with all the WordPress goodies we know and love (comments, categories, tags, etc.)
- Pages, Home page

All comments are within the PHP/Wordpress code, so none of it gets translated into the user’s browser or page source code. I even show you how to extend the function set I have included by default, so you can easily make the site more complex without learning anything extra.

```
<?php if ( have_posts() ) : 
 // Do we have any posts/pages in the databse that match our user's query (in the URL)?
 ?>
  <?php while ( have_posts() ) : the_post(); 
   // If we have a post to show, start a loop that will display it according to the formatting below
   ?>
````

If you like the sound of all this, why not [download the zipped theme](https://github.com/j-beckman/naked-wordpress/archive/master.zip) and [donate a dollar for the work](http://bckmn.com/pay)?
