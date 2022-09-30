# Sphinx-Pages-Template

Welcome to Sphinx-Pages-Template!

This is a template for creating Sphinx webpages hosted on Github Pages. 

## How to use

### Initial setup

First, create a fork of this template. Then, in your fork, change `ORGANIZATION_NAME` in `/.github/workflows/sphinx-build.yaml` to your Github username. Then, modify `/source/conf.py` to contain the proper author, copyright, and website name.

### Modifying the website

Then, edit the markdown files in `/source` to modify your website. When changes are committed, the website pages should autobuild into `/docs`. 

To add additional pages or change the layout of the sidebar, change `/source/index.rst` to match your layout.

To change the Sphinx theme, edit the variable `html_theme` in `/source/conf.py` to your theme's name, and add the name of the theme to `requirements.txt`. For a list of Sphinx themes, see [this page](https://sphinx-themes.org/).

### Deploying on Github Pages

In your repository settings (found at the top of the github page), find the Pages tab in the bottom left. Then, set "Source" to "Deploy from a branch," select a branch, and set the directory to `/docs`. After pushing a new commit, the page should update.
