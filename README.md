## styles-seed

### What is this is?

A starting point that I use for medium/large css projects.

Couple of notes:

- I've created it in SCSS and SASS.  If you prefer, Stylus, or even Less.  Feel free to convert it.
- The files are just suggestions, edit it to fit your taste.
- If you have any questions, don't hesitate to ping me.

### Structure
```
styles
|
|---lib                 // for reusing mixins and vars
|---mixins              // custom mixins
|---vars                // localized variables
|
|---global              // all reusable css is imported here
|
|---> global            // all modular css should have a home here
|   |---base
|   |---buttons
|   |---icons
|   |---layout
|   |---modules
|   |---state
|   └---typography
|
|---> vendor            // for storing vendor/library files
|
|---> modules           // for reusable module css
|   |---footer
|   |---header
|   |---forms
|
|---static              // for css that will only loades separately
|
|---ie                  // for that super fun part of writing ie only css

```

### Loading the files
The only required file to load is global.css.  I like to separate my
global from any static/singular css files so users can cache the more robust global folder.
Although, you shouldn't let it get very big anyway.

So load anything in ```/static/``` separately.

And ie.css is up to you.   These days, we need less and less in there.  But its there if you want it.

```
<link rel="stylesheet" href="styles/global.css">
<!--[if lte IE 8]><link rel="stylesheet" href="styles/ie.css"><![endif]-->
```

### Extra Files
This uses bower by default, although, its unnecessary.  If you do want to
use it, add this to your bower.json file

```
"devDependencies": {
    "semantic-grid": "*",
    "bourbon": "*",
    "normalize-scss": "*"
  }
```

And feel free to switch out Bourbon with Compass.

---------------------------

Inspired by (and uses):
- [SMACSS](http://smacss.com/)
- [Stubbornella](http://www.stubbornella.org/content/)
- [Twitter Bootstrap](http://getbootstrap.com/)
- [Normalize CSS](http://necolas.github.io/normalize.css/)
- [Semantic Grid](http://semantic.gs/)
- [Bourbon](http://bourbon.io/)
- [Bower](http://bower.io/)
- And a million other people doing amazing things

