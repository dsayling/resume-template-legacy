dockerized jsonresume
=====================

[![Build Status](https://travis-ci.org/dsayling/resume.svg?branch=master)](https://travis-ci.org/dsayling/resume)

## want to make your own resume from JSON?

Made with http://jsonresume.org

I suggest hosting with [github pages](https://pages.github.com/) since it's easy.

* just fork this repo
* rename to username.github.io
* clone and go!

You need to [install docker](https://docs.docker.com/install/).

# guide

* pick your [theme](https://jsonresume.org/themes/) and edit the Dockerfile with the theme; this uses [elegant](https://github.com/mudassir0909/jsonresume-theme-elegant)
 * update the `npm` package and the `-t` flag
* fill in the resume.json
* run the `./build` script
* push to your github.io page repo

## using github actions

An actions workflow is already setup. Simply edit the `resume.json` and push, then the workflow simply builds the html file (so you dont have to). If you push, said change to the `resume.json` to a branch titled `deploy`, it will push the generated html file to the `gh-pages` branch. Simply modify the workflow if you'd like to deploy to or from a different branch.

Thanks
======
Forked from https://github.com/BretFisher/resume
