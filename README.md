# What

A base set of SCSS stylesheets to start projects. No frameworks or learning curve, just a set of empty files to be customised as you need and a couple of handy mixins and functions.

## How

``gem install compass``

or

``gem install sass``

All the code is in the SASS folder. User config.rb to customise your settings if you will run **compass watch** (defaults to /stylesheets) or just run **sass --watch sass:[your css folder]** if you don't want the compass thing.

_In a Rails app you don't need compass, with the common sass-rails gem you are there. Just put this into the assets folder and call main.scss from your application.css file._

## The breakpoints

The grid has 4 breakpoints:

- 481up
- 768up
- 1030up
- 1240up
- 1600up

You can change the largest breakpoint easily in a variable called *$max-website-width* in the ``_grid.scss`` file. Well, you can do whatever you want ^__^

## Credits

This codebase has been curated by [https://github.com/xavib/](@xavi_b), and comes from several sources. Mostly based in [@eddiemachado's Bones](https://github.com/eddiemachado/bones) clever structure but there's also a little from [Zurb's Foundation](https://github.com/zurb/foundation) (the grid), and some other stuff coming from here and there.
