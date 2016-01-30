# What

A base set of SCSS stylesheets to start projects. No frameworks or learning curve, just a set of empty files to be customised as you need and a couple of handy mixins and functions.

We work with plain HMTL, Ruby on Rails and PHP projects at [season](http://www.season.es), so we've been working on a (really) simple structure for all scenarios.

## Why

In most cases, we use compass to compile SCSS. By doing it this way, we don't need to run _anyting_ in RoR projects, we can easily fit this with [middleman](https://middlemanapp.com/) for static sites and with tiny changes we can also easily integrate it with [Grunt](http://gruntjs.com/), [Glup](http://gulpjs.com/) or whatever.


## This thing at a glance

Directory         | Purpose
----------------- | ----------------------------------------------------------------------
`core`            | Core styles. Functions, mixins, font imports, variables...
`base`            | Holding the collection of high-level elements
`layout`          | Definition of the relationship between components
`component`       | Low-level elements
`vendor`          | Vendor files

## Some basic rules we trend to follow:

### Add media queries the closest to their component.

As an example, take a related news block. 4 columns and tag list in large viewports, 1 column without tag list in small viewports.

You would add the media query to show/hide the tag list in a file called ``component/_news--item.scss``

You would add the media query to fit the number of columns in a ``layout/_news--related.scss`` file.


## How (do we proceed)

Dependencies are managed via bundler. If you don't have it, run 

``gem install bundler``

Our common flow for starting a project is:

``bundle install``
``bundle exec compass watch``

## Credits

This codebase has been baked by [@xavi_b](https://github.com/xavib/) and is inspired by a bunch of lectures and conversations about structures.
