## Testing Production Site

All tests run against the staging server, by default.

If you need to run against the production site, include the --env parameter like this:

    grunt shell:continuous

    nightwatch

    nightwatch -c browserstack.json