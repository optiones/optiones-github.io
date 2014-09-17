## Use the Heroku button

1. Click the Deploy to Heroku button
2. Specify app name (optional)
3. Click 'Deploy for Free'

## Update deployment

First deployment to Heroku, after using the 'Deploy to Heroku' button:

    git push -f heroku master:master

For any subsequent updates, you can use the shorter:

    git push heroku master

## Deploy from command line

1. Make sure the [Heroku Toolbelt](https://toolbelt.heroku.com/) is installed
2. Open Terminal/Command Prompt.
3. Go to your binary-static directory
4. Run this: (where app-name is a custom name of your choosing)

        heroku create app-name

5. Check it is working:

        git remote -v

    you should see something like this:

        heroku git@heroku.com:app-name.git (fetch)
        heroku git@heroku.com:app-name.git (push)

6. Configure:

        heroku config:set BUILDPACK_URL=https://github.com/miyagawa/heroku-buildpack-perl.git
        heroku ps:scale web=1

7. Deploy:

        git push heroku master

8. Open site:

        heroku open