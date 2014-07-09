# Coding guidelines

## JSHint

We use JSHint to enforce certain coding principles.

[Description of JSHint Options](http://www.jshint.com/docs/options/)

[JSHint Error Explanations](http://jslinterrors.com/)

[JSHInt Default Options](https://github.com/jshint/jshint/blob/master/examples/.jshintrc)


## Strict Mode
Include at the beginning of each .js file:

    'use strict';

More details on strict mode:

[ECMAScript 5 Strict Mode, JSON, and More](http://ejohn.org/blog/ecmascript-5-strict-mode-json-and-more/)

[Strict Mode ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions_and_function_scope/Strict_mode)

[It’s time to start using JavaScript strict mode](http://www.nczonline.net/blog/2012/03/13/its-time-to-start-using-javascript-strict-mode/)

## Naming conventions

Variables that contain jquery selected elements should start with a '$'.

Not:

    var due = $('#due');

Do:

    var $due = $('#due');

## Anonymous closures

Use  always, to prevent global variables:

    (function () {
        // ... all vars and functions are in this scope only
        // still maintains access to all globals
    }());