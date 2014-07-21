# Angular Espresso

Start an app with AngularJS on the client, Express + Node + Socket.IO as your back-end, all written in CoffeeScript.

## Current version

Current version: 0.3.0

This version includes the following components:

* AngularJS 1.2.20
* Twitter Bootstrap 3.2.0
* Express 4.6.1
* LESS 1.7.3
* Socket.IO 1.0.6
* Jade 1.4.2
* UglifyJS 2.4.15
* Body Parser 1.4.3
* Serve Favicon 2.0.1

## Installation

You need to have installed [node](http://nodejs.org/), [CoffeeScript](http://coffeescript.org/), make sure
you install CoffeeScript globally. You also need [LESS](http://lesscss.org/).

Once you have them installed, extract the downloaded file, go to the directory it was extracted to and execute
setup.sh or setup.bat (depending on your OS):

## Cakefile Usage

Once you install the dependencies, use the Cakefile for performing different actions:
```
cake build                # Builds app
cake build:module         # Builds the Espresso module
cake build:client         # Builds client scripts
cake clean                # Clean module and client
cake clean:module         # Cleans the Espresso module
cake clean:client         # Cleans the client
cake run                  # Runs the app (you should build first)
```
The typical usage would be:
```
cake build
node app # or cake run
```
## Configuration

There's no configuration for using Angular Espresso, all you need to do is download the project, install its
dependencies with npm and run your node app.

Your .coffee files should be under the "app" folder. The project structure is the following:

NOTE: Each directory has a README file with more detail

* Angular: Your AngularJS app should go in this directory
* Services: Backend logic goes here
* Config: Configuration that may be used to set up different values for a specific environment or a common config
* Routes: This directory should contain the routing functions for your views. Define an entry point for a major
component of your site and then use partials for all its sub-components
* Resources: Any client scripts not related to AngularJS

At the root folder, there are two more folders to consider:

* Styles: Your LESS styles should go in this directory. Keep in mind that the project has Twitter Bootstrap already
included
* Views: Your views/partial views should go here

In the future, I will be adding support for testing. I won't implement file watching until it is stable in node.

## Contribute
If you want to help, fork/clone/share the project, suggest new features, and/or submit pull requests.
Contact me directly at [william.r.mora@gmail.com](mailto:william.r.mora@gmail.com) or [@_williammora](https://twitter.com/_williammora).

## Author
William Mora - [@_williammora](https://twitter.com/_williammora) - http://www.williammora.com

## References

For more on AngularJS: http://angularjs.org

For more on CoffeeScript: http://coffeescript.org

For more on Express: http://expressjs.com

For more on Jade: http://jade-lang.com

For more on Socket.IO: http://socket.io/

For more on LESS: http://lesscss.org/
