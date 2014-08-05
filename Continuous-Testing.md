## Testing Production Site

Continuous testing tests a huge list of URLs and checks for JavaScript or other errors. 
The list is compiled from the top 1000 visited URLs taken out of Google Analytics.

To run:

    grunt shell:continuous


Run with more options: go to /tests/continuous

Run locally:

    nightwatch

Run in BrowserStack:

    nightwatch -c browserstack.json