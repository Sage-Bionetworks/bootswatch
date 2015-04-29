Bootswatch
==========

Bootswatch is a collection of free themes for [Bootstrap](http://getbootstrap.com/). Check it out at [bootswatch.com](http://bootswatch.com).

Usage
-----
Download the `bootstrap.min.css` file associated with a theme and replace Bootstrap's default stylesheet.

The themes are also hosted on [BootstrapCDN](http://www.bootstrapcdn.com/).

Rails users should check out [twitter-bootswatch-rails](https://github.com/scottvrosenthal/twitter-bootswatch-rails).


Customization
------
Bootswatch is open source and you’re welcome to modify the themes.

Each theme consists of two LESS files. `variables.less`, which is included by default in Bootstrap, allows you to customize [these settings](http://getbootstrap.com/customize/#less-variables). `bootswatch.less` introduces more extensive structural changes.

These files are also available in SASS.

Synapse customized
-----
    Download this forked repo:  git clone https://github.com/Sage-Bionetworks/bootswatch.git 

    Synapse customizations to the paper theme are made in a branch version that corresponds to the bootstrap version that's being used in the product.
    At the time of writing, this is v3.3.2-customized

    Following the steps from [Bootswatch](https://bootswatch.com/help/) to configure npm and grunt.

    Build the bootswatch project to create a new bootstrap.min.css

    Rename bootstrap.min.css to bootstrap-paper-theme.min.css

    Replace the file in our gwtbootstrap3 project (gwtbootstrap3/src/main/resources/org/gwtbootstrap3/client/resource/css/bootstrap-paper-theme.min.css).

    Increase the gwtbootstrap3 project version, and rebuild.

    In SWC, update the pom to use the updated gwtbootstrap3 project version and rebuild.

    Verify that everything looks and functions correctly after the update!


API
-----

A simple API is available for integrating your platform with Bootswatch. Send your request to `http://api.bootswatch.com/3/`.

The swatch objects are returned in an array called `themes`, each one with the following properties:  `name`, `description`, `preview`, `thumbnail`, `css`, `cssMin`, `less`, and `lessVariables`.

More info at http://bootswatch.com/help/#api

Author
------
Thomas Park

+ http://github.com/thomaspark
+ http://thomaspark.me

Thanks
------
[Mark Otto](https://github.com/markdotto) and [Jacob Thornton](https://github.com/fat) for [Bootstrap](https://github.com/twitter/bootstrap).

[Jenil Gogari](http://www.jgog.in/) for his contributions to the Flatly theme.

[James Taylor](https://github.com/jostylr) for [cors-lite](https://github.com/jostylr/cors-lite).

[Corey Sewell](https://github.com/cjsewell) for SASS conversion.


Copyright and License
----
Copyright 2014 Thomas Park

Code released under the MIT License.
