## JSHint

We use JSHint to enforce certain coding principles.

[Description of JSHint Options](http://www.jshint.com/docs/options/)

[JSHint Error Explanations](http://jslinterrors.com/)

[JSHInt Default Options](https://github.com/jshint/jshint/blob/master/examples/.jshintrc)


## Nightwatch and Selenium

We use automated integration tests to protect against stability regression.

[Nightwatch](http://nightwatchjs.org/) can run tests against a local [Selenium](http://www.seleniumhq.org/) server or against [BrowserStack](http://www.browserstack.com/start)

These tests reside in
 
    /test/integration

In order to run the tests locally, you have to have [Selenium](http://www.seleniumhq.org/) server running on your machine.

To run the tests via [BrowserStack](http://www.browserstack.com/start) you need to specify your API keys via the command line (not yet implemented, but shouldn't be stored in the config).



Run all tests locally (on firefox):

    nightwatch

Run a single test:

    nightwatch -t tests/auth/loginFail

Run a group of tests:

    nightwatch -g auth

Run tests via BrowserStack:

    nightwatch -c browserstack.json

Run test on all browsers via BrowserStack:

    nightwatch -c browserstack.json -e chrome,firefox,ie


####You can also run via Grunt like this:

    grunt shell:nightwatch

or

    grunt shell:browserstack