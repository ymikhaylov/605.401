605.401
=======

Class project for 605.401

Setup
-----

Before running a server for the first time we need to install the app's
dependencies. Just run these two commands. (See the Tools section for
installing grunt and bower.)

    npm install    #get server side dependencies
    grunt install  #get client side dependencies

Building
--------

For development use

    grunt server

Which will open a web browser with the app and update it any time you save a
file.

For production mode use:

    grunt server:dist

Grunt will also run all the unit tests.

    grunt test

Tools
-----

Npm is the node package manager. It should be available in your distribution's
package manager (e.g. apt-get install npm) or you can install it manually
from http://nodejs.org/download/

Install grunt with:

    npm install -g grunt-cli

Install bower with:

    npm install -g bower

Layout
------

    .
    ├── app             #client side code
    │   ├── scripts     #javascript
    │   ├── styles      #css
    │   └── views       #html
    ├── design          #UML diagrams
    ├── lib             #server side code
    │   └── controllers
    ├── server.js       #server entry point
    └── test
        └── spec        #unit tests

Design
------

The UML design diagrams live in the design folder. To build them use:

    plantuml design/**.plantuml

Plantuml is available from http://plantuml.sourceforge.net/
