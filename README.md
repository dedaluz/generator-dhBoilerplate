# YO Generator dhBoilerplate

```
              dddddddd
              d::::::dhhhhhhh
              d::::::dh:::::h
              d::::::dh:::::h
              d:::::d h:::::h
      ddddddddd:::::d  h::::h hhhhh
    dd::::::::::::::d  h::::hh:::::hhh
   d::::::::::::::::d  h::::::::::::::hh
  d:::::::ddddd:::::d  h:::::::hhh::::::h
  d::::::d    d:::::d  h::::::h   h::::::h
  d:::::d     d:::::d  h:::::h     h:::::h
  d:::::d     d:::::d  h:::::h     h:::::h
  d:::::d     d:::::d  h:::::h     h:::::h
  d::::::ddddd::::::dd h:::::h     h:::::h
   d:::::::::::::::::d h:::::h     h:::::h
    d:::::::::ddd::::d h:::::h     h:::::h
     ddddddddd   ddddd hhhhhhh     hhhhhhh


   dhBoilerplate made with love & help.
   ---------------------------------------
   Author   :   David Hellmann
   Website  :   https://davidhellmann.com
   Github   :   https://github.com/davidhellmann/generator-dhBoilerplate
```


## Intro
That's my own YO Generator who fits for my own requirements.
Last year I go most of the time with CodeKit and a more oldsql workflow.
Now, this one is more up to date :)

Big thanks to [Sascha Fuchs](https://github.com/gisu) and his [Kittn](http://kittn.de/) for a lot of help and inspiration.
Also big thanks to [Martin Herweg](https://github.com/martinherweg) and his [YO Generator](https://www.npmjs.com/package/generator-mh-boilerplate) that help me a lot too.
And last but not least thanks to all members from our Slack Channel [webdevs](http://webdevs.xyz/) — feel free to join us.


## What is inside
### This three scenarios are covered by the generator:
- Prototyping (with Twig)
- WordPress with a basic Starter Kit (WordPress itself must be Installed by Hand after the first `gulp init`)
- Craft CMS with a basic Starter Kit (Craft CMS itself must be Installed by Hand after the first `gulp init`)

### Sass Functions
- `borderradius('level-x')` or `br('level-x')`
- `boxshadow('level-x')` or `bs('level-x')`
- `color('color-name')` or `c('color-name')`
- `ease('easing-name')` or `e('easing-name')`
- `fontfamily('font-name')` or `ff('font-name')` 
- `space(i)` or `s(i)`  
- `verticalrhythm(i)` or `vr(i)` 

### Sass Mixins
- `@include center`
- `@include clearfix`
- `@include container('full')` 'full' ist optional 
- `@include cols(i)`
- `@include filter(filter-name, value%)`
- `@include fluid-type($properties, $min-vw, $max-vw, $min-value, $max-value)` or `@include ft($properties, $min-vw, $max-vw, $min-value, $max-value)`
- `@include flexbox('full')` or `@include fb('full')` 'full' is optional
- `@include flexcols(i)` or `@include fc(i)`
- `@include fontsize('base', 1)` or `@include fs('base', 1)`
- `@include gutter(i)`or `@include g(i)`
- `@include pull(i)`
- `@include push(i)`
- `@include valign`
- `@include visuallyhidden` or `@include vh`


## Install
```
$ npm install -g generator-dhboilerplate
```


## Usage
Jump in your Working Directory and type:

```
yo dhboilerplate
```
Run through the options. When you're done grab a coffee. The node module installation take a while :)


## Install NPM Packages

```
npm install // yarn install
```


## Initialize Project

```
gulp init  // npm run init OR yarn init
```


### Default Task with BrowserSync

```
gulp // npm run dev OR yarn dev
```


### Task for Building
This Task clean the folder, build the stuff from ground up and optimize the images and minifiy JS / CSS files. Ready for live!

```
gulp build // npm run build OR yarn build
```


### Other Tasks
There are some other Tasks there…

```
// NPM RUN / YARN COMMANDS
"start": "gulp init",
"dev": "gulp",
"build": "gulp build",
"criticalcss": "gulp criticalcss",
"clean:dist": "gulp clean:dist",
"clean:templates": "gulp clean:templates",
"clean:images": "gulp clean:images",
"clean:js": "gulp clean:js",
"clean:css": "gulp clean:css",
"copy:fonts": "gulp copy:fonts",
"copy:images": "gulp images",
"copy:favicon": "gulp favicon",
"copy:svg": "gulp svg",
"copy:single": "gulp svg-single",
"copy:sprite": "gulp svg-sprite",
"copy:sysfiles": "gulp systemFiles",
"copy:templates": "gulp templates"

// Clean Tasks
// Clean the specific folder in the "___dist" dir
gulp clean:templates
gulp clean:css
gulp clean:js
gulp clean:images


// Main Tasks
// All this are triggered within "gulp init" & "gulp build" task.
// Some of this are triggered within the "gulp" task.
gulp templates
gulp systemFiles
gulp modernizr
gulp compile:js
gulp sass
gulp copy:fonts
gulp images
gulp svg-single
gulp svg-sprite


// Minify Tasks
// This task are triggered within the "guld build" task.
gulp minify:js
gulp minify:sass
gulp minify:images

```

## Thanks to
- webdevs - for so many things: [Website](http://webdevs.xyz)
- Sascha Fuchs - for help help help: [Website](https://github.com/gisu)
- Martin Herweg - for help help help: [Website](https://github.com/martinherweg)
- CSS Tricks -  for Easing Map: [Website](https://css-tricks.com/snippets/sass/easing-map-get-function/)
- Florian Kutschera - for the Material Design Box Shadows: [Website](https://medium.com/@Florian/freebie-google-material-design-shadow-helper-2a0501295a2d#.f1fz5ac2o)
- Hugo Giraudel & Eduardo Bouças - for include media: [Website](http://include-media.com/)
- @LukyVj - for family.scss: [Website](http://lukyvj.github.io/family.scss/)
- inuitcss - for some snippets and inspiration: [website](https://github.com/inuitcss/inuitcss)

[![bitHound Overall Score](https://www.bithound.io/github/davidhellmann/generator-dhBoilerplate/badges/score.svg)](https://www.bithound.io/github/davidhellmann/generator-dhBoilerplate)
