# Drupal Project Setup

##Purpose 
In order to help your Drupal project succeed, we've put together a helpful page to help you track down your project's 
resources, find out what to build, and relevant Drupal documentation. 

## Hosting choices
[@TODO: Write about how hosting destination matters.  Git repos.]

## Getting the Code
[@TODO: List dev, staging, QA, etc.]

### Recommended Project Structure
[@TODO: List dev, staging, QA, etc.]

### External Environments
[@TODO: explain this section, provide placeholders for assets]

### Branching Strategy

## Mainframe Systems Page for Credentials


## API Documentation
See https://api.drupal.org/api/drupal for complete documentation on various version of Drupal core.  

## Coding Standards
[@TODO: Talk about Drupal's varient of our Coding Standards ]
Drupal's coding standards are specified [here](https://www.drupal.org/coding-standards)

Main differences between Drupal's coding standards and standard Nerdery coding standards are:
* 2 spaces instead of 4 for indentation.
* 

You can use phpstorm's Drupal plugin to configure your project with Drupal's coding standards

## Deployment ##
Here are some helpful tips for how to us the drush command line tool for deploying Drupal sites.

1. Export your whole site: 
```drush arb  --destination=/root/prod-201510061.tar.gz```
 
2. Export your whole site without including the files:
```drush arb --tar-options="--exclude=%files" --destination=/root/prod-201510061.tar.gz```
 
3. Export just the database:
