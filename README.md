TopShelf is a modern boilerplate with Bourbon, Neat, Bitters & extras, chilled with Normalize, jQuery & Modernizr.

It enables you to hit the ground running with clean, semantic coding. It's designed for use with Mixture, but can be adapted to other projects near trivially.

Read more below or clone this repository and get right to work.

USING TOPSHELF
==============

## 1. Before You Begin

### 1a. General Info

TopShelf is built for use with [Mixture.io](http://mixture.io) first and foremost. If you're planning on using it with Mixture as intended, clone the repository and you'll be ready to get to work. There are a few TODOs included to get yourself started.

**Debug Mode is turned on by default**

Debug mode will use your unminified assets during testing and will leave comments intact. You can disable this by turning "debug" from true to false inside "mixture.json" in the project root.

 **Are you on Windows?**
 
Mixture as of this writing has libsass disabled in Windows. It's enabled by default in this project(simply because it's faster), but can be disabled by changing "uselibsass" from true to false inside "mixture.json" in the project root.

**Looking to use Topshelf without Mixture?**

If you're looking to use this boilerplate without Mixture(like with Grunt/Gulp/Yeoman etc), you can certainly do so. You'll need to remove the ".mix" specific JS file inside inventory and bring your own HTML/templates. You can continue to use the Liquid templating system, but you'll need to have a plugin for that inside your preprocessor file. You'll get all the benefits of the Bourbon.io stack, as well as all the TopShelf goodies.

### 1b. What's included?

#### [Bourbon](http://bourbon.io):

Bourbon is a library of pure Sass mixins that are designed to be simple and easy to use. No configuration required. The mixins aim to be as vanilla as possible, meaning they should be as close to the original CSS syntax as possible.

#### [Bourbon Neat](http://neat.bourbon.io):

Neat is a semantic grid framework built on top of Sass and Bourbon. It is simple enough to get you up and running in minutes, and powerful enough to handle any responsive layout you can dream of.

#### [Bourbon Bitters](http://bitters.bourbon.io):

Bitters helps designers start projects faster by defining a basic set of Sass variables, default element style and project structure. It’s been specifically designed for use within web applications. Bitters should live in your project’s root Sass directory and we encourage you to modify and extend it to meet your design and brand requirements.

#### [Bourbon Refills](http://refills.bourbon.io):

Components and patterns built with Bourbon and Neat.

#### [Garnish (for Bourbon)](https://github.com/paulozoom/garnish):

Garnish is a collection of Sass mixins and functions designed to make your life a tiny bit easier.

####[Chasers (for Bourbon)](https://github.com/kennethormandy/chasers):

Collection of Bourbon Neat helpers.

#### [Modernizr-mixin](https://github.com/danielguillan/modernizr-mixin):

A simple way for DRYier, faster and cleaner Modernizr tests in Sass.

#### [Bower](http://bower.io):

A package manager for the web

#### The usuals:

All your favorites are included. That means [normalize.css,](http://necolas.github.io/normalize.css/) [jQuery,](http://jquery.com) [modernizr,](http://modernizr.com/) [FontAwesome(as a mixin!)](http://fortawesome.github.io/Font-Awesome/), and [html5boilerplate](https://html5boilerplate.com/) are all included to give you the ultimate starter toolkit.

#### TopShelf Extras:

Don't bother including a giant stylesheet just to be able to call easy to remember icon names. Use FontAwesome shorthand names with the included icon mixin and keep your CSS clean. Want to use another icon set? Bring your own set and only include what you need! Also included is a powerful button generator that allows you generate modern-looking buttons with various styles, automatic font color, rounded corners and even automatically positioned icons!

### 2. Terminology / File Structure

#### 2a. Root Folders

TopShelf tries to maintain a clean base file structure. All your finished, production ready code is placed into /assets/ by Mixture, while all your work in progress / uncombined files reside in /inventory.

**/inventory/**

Inventory is the folder where all of the CSS, SASS, and JS files reside. This folder contains all of our recipes, ingredients and specials, all of which you'll read about in a minute.

**/menu/**

Pages, templates and layouts are stored here. These files are the pages/layouts "on the menu" for Mixture to serve up to the user.

**/models/**

The models folder contains json files that contain data that is stored for use by the Liquid templating system that Mixture uses by default. The data inside these files can be used in extremely powerful and robust ways.

**/assets/**

This folder will be initially empty of any real files when you download TopShelf. Files will automatically be added inside this folder with your combined css files, combined javascript files and include their minified versions as well. All images should also be placed in the /assets/images.

#### 2b. Topshelf Nomenclature

TopShelf uses some bar related terms for our file/folder structures that I find helpful in daily use.

/inventory/**recipes/**

All good drinks start with a recipe, and with TopShelf, it's no different. We include all of our bower-ready components in this file and import them later.

/inventory/**ingredients/**

Ingredients are what give our site style and flavor. Topshelf's extras, as well as site branding_(_ambiance.scss)_ and grid/structure are included here. You should place any widely used component styles in their own files/folders here, like _/ingredients/_navigation.scss._

/inventory/**specials/**

Specials are where we store our page specific styles / page specific components.

/inventory/**bartender.scss**

The bartender.scss file is responsible for mixing all of our recipes, ingredients and specials together and making a final product. We import Bourbon, Neat, Biters and all of our extras here first. Then we setup our grid, pass in our ambiance / structure files. This will be generated into _/assets/bartender.css_. Feel free to rename for your project.

/inventory/**barback.mix.js**

This special .mix file allows us to import multiple JS files into one finalized JS file to reduce HTTP requests / clutter. By default, jQuery and Modernizr are combined. Feel free to rename for your project.

**Still having trouble?** [Submit an issue](https://github.com/qburns/topshelf/issues) on github and I'll try to help.

    Thanks to @89yesler for idea on naming convention/some file structure things.


## Github page 
https://github.com/qburns/topshelf


