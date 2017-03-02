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

## Troubleshooting

### Common Errors

If you see this error, you probably have a syntax error within your markdown files that need to be corrected.

``` shell
There were errors during this build, re-run with `middleman build --verbose` to see the full exception.
```

You can refer to these pages for examples:

	* [Markdown syntax used in Slate](https://github.com/lord/slate/wiki/Markdown-Syntax)
	* https://daringfireball.net/projects/markdown/
	* http://www.markdowntutorial.com/

You can also copy and paste your markdown code here to get a live translation of how it outputs. You can look through the output to detect your syntax error.

	* http://dillinger.io/

