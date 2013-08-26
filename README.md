## adamin-style-seed

### What is this is?
Just a starting point that I recreate all to often when setting up projects
Its my mixture of resources that I use when prototyping and designing

I've grown to like it.  And I'll probably keep updating it as time goes by.

Couple of notes:

- Its all in SASS.  If you like SCSS, Stylus, or even Less.  Feel free to convert it.
- If you want to use it, the files are just suggestions, do with it what you like.
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
|---> libraries         // for storing vendor/library files
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

### Bower
This uses bower by default, although, its far from necessary.  If you do want to
use it, add this to your bower.json file

```
"devDependencies": {
    "semantic-grid": "*",
    "bourbon": "*",
    "normalize-scss": "*"
  }
```

Inspired by (and uses):
- [SMACSS](http://smacss.com/)
- [Stubbornella](http://www.stubbornella.org/content/)
- [Twitter Bootstrap](http://getbootstrap.com/)
- [Normalize CSS](http://necolas.github.io/normalize.css/)
- [Semantic Grid](http://semantic.gs/)
- [Bourbon](http://bourbon.io/)
- [Bower](http://bower.io/)
- And a million other people doing amazing things

