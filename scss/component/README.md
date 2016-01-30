# Component Partials

Consider a component anything that should have the same styling definition regardless of their location between the layout.

Consider some hierachy here, for better mantainance.

Take as an example a news item element. You could do something like:

File                  | Purpose
--------------------- | ---------------------------------------------
`_news.scss`          | Compile all news components, that may hold common news item styles. Let's say text color. This is what we will call in the main stylesheet.scss
`_news--promoted.scss`| Specific news promoted display styling
`_news--teaser.scss`  | Specific news teaser display styling
`_news--detail.scss`  | Specific news detail page styling

> Ieah, it's a bit drupalish-displaysuiteish. But one of the good things of Drupal is that gives a clear name to almost everything. Makes sense to take advantadge of that everywhere, huh?