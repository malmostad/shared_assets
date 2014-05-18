Common Assets
=============

Sass variables, mixins, extends and functions that are shared between projects to build CSS files for The City of Malmo. Not to same as the [Global Assets](malmostad/global_assets) that you include in your applications web pages when they are served.

## Usage
Add the files to you git project and update them with [Bower](http://bower.io/) (recommended). It’s also possible to use [npm](https://www.npmjs.org/) or [Git submodule](http://git-scm.com/book/en/Git-Tools-Submodules).

### With Bower

Install [Bower](http://bower.io/) if it’s not already on your development system.

Run:

    bower install malmostad/shared_assets

Add the files to your git repository.

To update the shared asset files, run:

    bower update

## Use the files
Add `external_malmo.scss` to the top of your own main Sass file:

    @import 'malmo_external';

Or if `external_malmo.scss` is not in your Sass load path, point to it with a relative path, e.g.:

    @import '../vendor/malmo_shared_assets/malmo_external';


### Change the default bower directory
The default directory for Bower modules is `bower_components` in your project root. If you want to use a custom install directory, e.g. `vendor`, add a `.bowerrc` file to your project’s root:

    {
      "directory": "vendor"
    }


## License
Released under AGPL version 3.
