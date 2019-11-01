# Handlebars.js

> Handlebars is a JavaScript library that enables the creation of standardized HTML templates within JavaScript. Through its use one can write cleaner code by following the separation of concerns principle of  computer science.

## Using Handlebars.js
* Like any other library, Handlebars.js can be included locally or be delivered via CDN.

* To prevent your interpreter from attempting to parse Handlebars scripts as vanilla js you must include a type attribute of the script tag: type="text/x-handlebars-template"

* Handlebars templates contain HTML and text along with expressions to be evaluated by Handlebars. 

* Handlebars expressions are contained within {{ }} or {{{ }}} [Moustaches](https://mustache.github.io/)

* {{ }} represents HTML escaped by Handlebars

* {{{ }}} represents raw HTML

* Handlebars has the context of the JavaScript Object that is passed. It also has built-in block helpers that can change that context.
  - For example, #each will iterate a list that matches the expression it precedes.
  - #if will allow conditional execution of an expression.

* Helpers can take the format of standard helpers or block helpers.
  - Helpers can be created with the built-in registerHelper function.
  - There are a number of built-in helpers
  - Helpers can accept parameters
  - Block helpers require a closing tag.
    + When creating a block helper one must use the second parameter of the registerHelper function. This *options* parameter grants access to additional properties necessary for the block helper.

* Use of a template tag can replace the use of a script tag and may demonstrate intent better.
## References
[10-Min Tutorial](https://tutorialzine.com/2015/01/learn-handlebars-in-10-minutes)

[Handlebars.js Documentation](https://handlebarsjs.com/)
