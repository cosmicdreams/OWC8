# Bacon Project Doc Boilerplate

## Purpose
Use the boilerplate docs in this folder as a starting point for your project documentation.

## Boilerplate Updates
Anyone is welcome to make changes to these boilerplates, but please do so in a feature branch so they can be reviewed before merging.

## Setting up MDwiki in your project
To get these docs working in your project, just copy/paste the contents of this directory into your project. If for some reason you need to keep these docs internal, you can add them above your web root and configure a separate vhost entry (ex. mysite-docs.com) to give you more control over permissions.

## MDwiki Primer

### index.html
This is where all the magic happens. Unless you're wanting to adjust the theme of your documentation you never need to touch this file.

### config.json
Currently, we're only using this to set the \<title\> tag for the documentation. See the MDwicki docs below for more config options.

### index.md
This is what gets loaded by default if a specific page isn't requested in the URL.

### navigation.md
This is used to stitch together the markdown files into a pretty top-nav. This is also where you specify the site title the appears in the top left of the page.

### All other .md files (ex. development.md)
These files will represent the different sections of your documentation. Some boilerplates have been provided to give you an idea of how you can organize your docs into internal and client-facing sections. Files can also be organized into directories if needed.

## More MDwiki Info
- [MDwiki Documentation](http://dynalon.github.io/mdwiki/#!index.md)
- [MDwiki GitHub](https://github.com/Dynalon/mdwiki/)