# EJS
> EJS => Embedded JavaScript

EJS is a templating language used to dynamically render HTML and is written with common JavaScript syntax.

To use EJS for templating within express first one must set the express view engine to EJS:

    app.set('view engine', 'ejs');

After this initial step in any application routes you can include the statement: 

    response.render('PATH TO EJS FILE', {OBJECT WHOSE PROPERTIES PROVIDE VARIABLE ACCESS});

substituting appropriately the ALL-CAPS.

The advantage of using a templating engine is the same as the advantage of using a template in any context. Saving time by introducing automation into repetitive tasks. 

Within the EJS files there is a wide spectrum of functionality. You can include other EJS files as partials, composing them together to make whole documents. Or you can make HTML dependent on processed data to directly align design with function. 



# References 
[More information on View Engines within Express](https://expressjs.com/en/guide/using-template-engines.html)

[Cheatsheet](https://onecompiler.com/cheatsheets/ejs-embedded-javascript-templates)

[Video Tutorials](https://www.youtube.com/playlist?list=PL7sCSgsRZ-slYARh3YJIqPGZqtGVqZRGt)