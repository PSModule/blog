# Template-Blog

A template repo for blog repositories.

## Prerequisites

1. New branch called 'gh-pages' created from the main branch.
2. Enable GitHub Pages in the repository settings, selecting the 'gh-pages' branch as the source.
3. Enable Discussions in the repository settings.

## Deploying the blog

The `Blog.yml` file is used to deploy the blog to Github Pages. The entire blog is generated from the discussions in the repository and runs
when . The workflow is triggered when a discussion is created or updated.


## Deploying a blog post

1. Open a Discussion of type 'Blog'.
2. Upon [discussion creation of update, a workflow is triggered](https://docs.github.com/en/actions/writing-workflows/choosing-when-your-workflow-runs/events-that-trigger-workflows#discussion):
   - Get all discussions of type 'Blog'.
   - Create a Markdown file for each discussion.
   - Push the Markdown files to the 'gh-pages' branch.
3. GitHub Pages will automatically deploy the changes to the website.
