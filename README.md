# Point guard

A boilerplate for Sass and JavaScript.

**What you'll need**: [Ruby](http://www.ruby-lang.org), [Gem bundler](http://gembundler.com/), [rvm](https://rvm.io), [node](http://nodejs.org), [npm](https://npmjs.org), [Sass](http://sass-lang.com/), [Bourbon](http://bourbon.io), [Bourbon Neat](http://neat.bourbon.io), [Guard](https://github.com/guard/guard), [Bower](http://bower.io), [pow](http://pow.cx), [livereload browser extension](http://feedback.livereload.com/knowledgebase/articles/86242-how-do-i-install-and-use-the-browser-extensions-)

- - - 

## Setup

Clone the repo

    git clone https://github.com/joshfry/point-guard.git

Rename the project, for example, "myapp"

    mv point-guard myapp

cd into "myapp"

    cd myapp

Download required gems

    bundle install

cd into scss directory
    
    cd scss
    
install Bourbon
    
    bourbon install
    
install Bourbon Neat
    
    neat install
    
Go back to project root
    
    cd ..
    
Install project dependancies with Bower

    bower install
    
Create a webserver with powder using pow to host project files located at myapp.dev

    powder link
    
Run guard to compile sass, concat js and livereload the browser when changes are made to any file

    guard

### All the above in one command

    echo What is the name of your project? ; read NAME ; git clone https://github.com/joshfry/point-guard.git && mv point-guard $NAME && cd $NAME && bundle install && cd scss && bourbon install && neat install && cd .. && bower install && powder link && open http://$NAME.dev && guard

## Bower

Bower packages are installed in the `/js/components/` directory. The configuration is handled with the `.bowerrc` file.

To add a new package

    bower install <name-of-package> --save

To uninstall a package

    bower uninstall <name-of-package> --save

## Guard Concat

Edit `Guardfile` to add the js files you want to concat and in which order.
