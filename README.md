Shared Assets
=============

Sass variables, mixins, extends and functions that are shared between projects to build CSS files for The City of Malmo. Not to same as the [Global Assets](https://github.com/malmostad/global_assets) that you include in your applications web pages when they are served.

See the *Gettings Started* and *Grids and Responsive Design* sections of the [Web Application Guidelines](http://malmostad.github.io/wag-v4) for usage.

## Usage
Use [Bower](http://bower.io/) (recommended) to add the files to your git project and keeping them updated. It’s also possible to use [npm](https://www.npmjs.org/) or [Git submodule](http://git-scm.com/book/en/Git-Tools-Submodules).

### With Bower

Install [Bower](http://bower.io/) if it’s not already on your development system.

Add the shared assets to your project with the following command:

    bower install malmostad/shared_assets

To update the shared asset files, run:

    bower update

### Change the default bower directory
The default directory for Bower modules is `bower_components` in your project root. If you want to use a custom install directory, e.g. `vendor`, add a `.bowerrc` file to your project’s root with the following JSON configuration:

    {
      "directory": "vendor"
    }

## Use the Sass files
Add `malmo_external.scss` or `malmo_internal.scss` to the top of your own main Sass file:

    @import 'malmo_external';

Or, if `malmo_external.scss` is not in your Sass load path, point to it with a relative path, e.g.:

    @import '../vendor/malmo_shared_assets/stylesheets/malmo_external';


## License
Released under AGPL version 3.
