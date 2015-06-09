# Lodepen - Minimal local front-end playground

I love [Codepen](http://codepen.io) but local performance is much better after all, that's why I've created this to serve as *local Codepen*.

## Advantages

* Sync across multiple browsers / machines (yes! you can sync to your phone for example) instantly upon save (thanks to [Browsersync](http://www.browsersync.io)) 
* Automatically complies pre-processors like Jade and Stylus
* Debug on Browser dev tools without the extra wrappers from Codepen's site
* Add jQuery, AngularJS, etc with bower, giving much more flexibility

## Install

Just clone or download zip for now ...

Assuming you have [node](https://nodejs.org), [npm](https://www.npmjs.com), [bower](http://bower.io) and [gulp](http://gulpjs.com) installed

After the repo is downloaded, to start, run `npm install`, `bower install`, and then `gulp` for serving and syncing

Default browser should automactically open and go to `http://localhost:3000`. To view it on other machines, see the External URLs in the console messages once server is up.

## File Structures
### Example
```
├── dist/
├	├── style.css
├	└── script.js
├── lib/
├── node_modules/
├── src/
├	├── index.jade
├	├── script.js
├	└── style.styl
├── index.html
├── *.others
```
### Important folders
**src/** contains the original code for **html**, **css**, and **js**, just like what you'd have on Codepen, I'd suggest keeping it simple with just 3 files but there's nothing stopping you from adding more.

Compiled **index.html** is located in the **root** folder. **Css** and **js** are located in **dist/**, that's where you'd link them

Bower libraries are within **lib/** and that's where you'd find and link them

That's pretty much it!

## License
MIT