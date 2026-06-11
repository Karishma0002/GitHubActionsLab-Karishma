# GitHubActionsLab-Karishma

## Purpose of the Workflows

In this lab, I practiced using GitHub Actions to understand how workflows can automate tasks in GitHub. I created workflows to learn how jobs can either run one after another or run at the same time.

## Workflow 1 – Job Dependencies

For the first workflow, I created three jobs:

* Build
* Test
* Deploy

I used the `needs` keyword so the jobs run in order. The build job runs first, then testing starts after build finishes, and deployment runs after testing is completed.

This workflow runs whenever changes are pushed to the main branch.

## Workflow 2 – Multi Platform Testing

For the second workflow, I created three jobs to run on different operating systems:

Ubuntu
Windows
macOS

Each job checks out the repository, displays system information, and creates a small file to show that the workflow is running correctly.

Since there were no dependencies between jobs, all three jobs ran at the same time.

This workflow runs when a pull request is created to the main branch.

## Key Concepts Demonstrated

 `needs` → used to make jobs depend on each other.
 `runs-on` → used to choose the operating system for each job.
 `actions/checkout@v4` → used to access repository files during workflow execution.

## Challenges Faced

One challenge was understanding when workflows trigger and making sure they ran successfully. Another challenge was understanding the difference between dependent and independent jobs. After testing the workflows and checking the Actions tab, I was able to understand how they work and complete the lab successfully.
