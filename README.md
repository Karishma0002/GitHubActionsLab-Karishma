# GitHubActionsLab-Karishma

## Purpose of the Workflows

In this lab, I practiced using GitHub Actions and learned how workflows can automate tasks in GitHub.

## Workflow 1 – Job Dependencies

For this workflow, I created three jobs:

* Build
* Test
* Deploy

I used `needs` so the jobs run in sequence.

This workflow runs when changes are pushed to the main branch.

## Workflow 2 – Multi Platform Testing

For this workflow, I created three jobs:

* Ubuntu
* Windows
* macOS

These jobs run independently and execute at the same time.

This workflow runs when a pull request is created.

## Key Concepts

* `needs`
* `runs-on`
* `actions/checkout@v4`

## Challenges Faced

One challenge was understanding how workflows trigger and how dependent and independent jobs work. After testing and checking the Actions tab, I was able to complete the workflows successfully.
