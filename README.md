# Learn a [Jamstack](https://jamstack.org/) 

## See the result

https://main--cranky-ride-6119ee.netlify.app/

## What am I doing?

Trying out a Jekyll+NetlifyCMS Jamstack (think full-stack, but awesome) [based on this project](https://github.com/adamwatters/jekyll-tutorial-with-netlify-cms/tree/master) but with a few important fixes:
1. admin/_config.yml, line 5   --> branch: main
2. admin/_config.yml, line 58  --> name: "layout",

## To replicate this project
You'll need a Netlify account. It serves three primary purposes:
1. Deploys website [shown here](https://main--cranky-ride-6119ee.netlify.app/)
2. Integrates with GitHub for seamless CI/CD
3. Lets you log in and add blog posts using a graphical web interface thru the NetlifyCMS admin panel as a guest (instead of requiring a developer to get involved - no source code modifications required! Pretty nifty, eh?)

## Protips

I used VSCode - if you clone the repo use the Remote Development extension to open the source code in a Jekyll container.
To test locally inside a containerized environment, run the following commands inside the container (i.e. by using the VSCode terminal or Docker CLI):
1. bundle install
2. bundle exec jekyll serve

Then open [localhost:4000](localhost:4000) in your browser.

This way when you're done and ready to clean up after yourself, just kill the container.
