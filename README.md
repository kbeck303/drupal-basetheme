# Oomph Origins
Origins uses modern technologies but has options to add in fallbacks for those less fortunate browsers. The particular client requirements will drive the actual process but Origins includes a great starting point for rapid theme development.

## Technologies

### Sass
Website: [http://sass-lang.com/](http://sass-lang.com/)

Configuration file can be found at:
* root > sass > _config.scss = order of files
* root > gulpfile.js = compiler settings

### Gulp
Website: [http://gulpjs.com/](http://gulpjs.com/)

Configuration file can be found at:
* root > gulpfile.js = gulp functions
* root > package.json = module dependancy list

Install Directions:
* cd into your theme directory
* run $ npm install = this will install the module dependancies listed in the root > package.json
* a new folder called "node_modules" will be created in your theme folder

We added a script to the root > package.json file to remove all ".info" files within the "node_modules" folder, which was causing errors on admin pages and when trying to run drush commands

In order to use gulp you will have to install [node.js](http://nodejs.org) on you system. This article is a great tutorial on how to get up and running quickly. [Getting started with Gulp](travismaynard.com/writing/getting-started-with-gulp)

### Susy
Website: [http://susy.oddbird.net/](http://susy.oddbird.net/)

Configuration can be found at:
* root > sass > _config.scss = grid configuration

### Compass
Website: [compass-style.org](compass-style.org)

Configuration can be found at:
* root > config.rb = compass configuration

## Support
This theme supports modern browsers - so IE9+. If you project requires IE8 support their are options availble to help with that.

[Modernizr.js](modernizr.com) is used for feature detection. It also ships with html5shiv.js which enables HTML5 elements in IE.

[Respond.js](https://github.com/scottjehl/Respond) is a library that allows IE6-8 to read media queries which is essential since we are using a grid system. This should only be loaded conditionally if you are trying to support those browsers.

[Pixrem](https://github.com/gummesson/gulp-pixrem) is a Gulp plugin that is used to convert REM units into pixels for IE fallbacks.
