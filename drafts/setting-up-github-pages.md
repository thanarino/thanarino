---
layout: post
title: Setting up a GitHub Pages-based blog site
categories: dev
---

This should have been the first post since I should have fixed most of the bugs before deploying this to "production" but hey at least I fixed them :) :) :)

Also, this is not a step-by-step guide on how to set up, but rather a list of "things to remember" containing issues I ran into when setting up. My set up involves a GitHub pages deployment of a repository, so there is a `/project-name` appended to my `thanarino.github.io`.

## Techs

### Jekyll

Jekyll is a static site generator, written in Ruby, that converts markdown into _legit_ website posts. More information is in the official Jekyll Quickstart [guide](https://jekyllrb.com/docs/). The thing to remember here is that when running `bundle exec jekyll serve`, if using a GitHub pages deployment of a project, use `bundle exec jekyll serve --baseurl=''` as a run command to remove the configured baseurl property in the _config.yml file.