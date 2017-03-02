---
# Publishing Your Docs


## Publish Locally

In order to publish your documentation locally and view the output run:

``` shell

bundle exec middleman build --clean

```
Then go into your **slate>build** folder and view index.html in your browser.

## Publish to Github

Publishing your API documentation couldn't be more simple. Make sure your origin is a Slate fork in your own account, not our original repo. 

Run the following command lines:

``` shell
# Initialize git
git init
# Add all the files
git add .
# Your first commit
git commit -m "First commit”
# Commit your changes to the markdown source
git commit -a -m "Update index.md”
# Push the markdown source changes to Github
git push
# Run the deploy script
./deploy.sh

```

Done! Your changes should now be live on http://lizchang617.github.io/slate, and the main branch should be updated with your edited markdown. Note that if this is your first time publishing Slate, it can sometimes take ten minutes or so before your content is available online.