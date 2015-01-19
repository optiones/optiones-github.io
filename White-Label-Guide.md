The Binary.com White Label program allows affiliates to create their own branded versions of the Binary.com platform.

This is a tech guide on how to implement the branded version. 
For a high-level overview of what our White Label program is, [read here](https://www.binary.com/white-labels).

## Initial Setup

Start by forking this repository. Then follow the steps described in [Initial Setup](Initial-Project-Setup)

## Project Organization

There are only few folders you need to focus on, in order to fully customize the site's look and feel to your needs.

#### Images folder

The folder contains the logo and other branding and miscellaneous image resources.

#### Sass folder

This is where all styling resides. We use SASS to better manage the styling process.

You would want to start with the _constants.scss file, which contains many base variables like colors, font sizing, and common control element sizes.

#### Templates folder

The folder contains all the templates from which the site's html is generated. You will need to change the relevant files in order to change branding and content.

    templates\haml - contains templates in [HAML](http://haml.info/) format

    templates\toolkit - contains templates using [Template Toolkit](http://www.template-toolkit.org/)

## Test Deployment
To be able to see how the pages look when rendered, you can create a free installation on Heroku.
Follow the [Heroku Deployment Guide](Heroku-Deployment)


#### JY:

Company name - should we allow/force them to change? should they keep part of the branding? I am assuming they will be able to change the logo and the name completely?

License logos and legal copy - is it mandatory it is left as-is?