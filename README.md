Jenkins Drupal template
=======================

A basic template for setting up Drupal testing/code analysis jobs in Jenkins.

Based on https://github.com/reload/jenkins-drupal-template


Installation
------------

### Setting up your project

To use this project, your project must include the build file from the [phing-drupal-template](https://github.com/reload/phing-drupal-template) project, either directly or as a submodule.

### Setting up Jenkins

1. Copy this directory to `/var/lib/jenkins/jobs/drupal-template`.
2. Create a new job and select *Copy existing job*, enter `drupal-template` in the *Copy from* field.
3. Uncheck the *Disable Build* checkbox
4. Configure the *Source Code Management* build step to check out a copy of the repository containing your Drupal project.


Requirements
------------

To use this template in Jenkins you must install the following plugins:

* analysis-core
* checkstyle
* dry
* phing
* plot
* pmd
* envinject
* warnings
* greenballs
* xvfb