# Coding guidelines

## Anonymous closures

Use  always, to prevent global variables:

    (function () {
        // ... all vars and functions are in this scope only
        // still maintains access to all globals
    }());


## Strict Mode
Include at the beginning of each .js file:

    "use strict";

It is important that each statement is put in a closure like this (so the strict mode does not extend when bundling to files that are not intended):

    (function(){
        "use strict";

        // All other code here
    })();

More details on strict mode:

[ECMAScript 5 Strict Mode, JSON, and More](http://ejohn.org/blog/ecmascript-5-strict-mode-json-and-more/)

[Strict Mode ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions_and_function_scope/Strict_mode)

[It’s time to start using JavaScript strict mode](http://www.nczonline.net/blog/2012/03/13/its-time-to-start-using-javascript-strict-mode/)

## Naming conventions

Variables that contain jquery selected elements should start with a '$'.

Don't:

    var due = $('#due');

Do:

    var $due = $('#due');