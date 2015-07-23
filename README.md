metalsmith-date-in-filename
====

Enrich file metadata with date info present in source filenames.

[![Build Status](https://travis-ci.org/sanx/metalsmith-date-in-filename.svg?branch=master)](https://travis-ci.org/sanx/metalsmith-date-in-filename)
[![npm version](https://badge.fury.io/js/metalsmith-date-in-filename.svg)](http://badge.fury.io/js/metalsmith-date-in-filename)

Installation
----

`npm install --save-dev metalsmith-date-in-filename`

Usage
----

Set the date in the filename:

    2014-11-04-file.md
    date-can-2014-11-04-go-anywhere.md
    like in parenthesis (2014-11-04).md
    20141104-compact-format.md
    compact-20141104.md

Then in your code:

    var Metalsmith = require('Metalsmith');
    var dateInFilename = require('metalsmith-date-in-filename');
    Metalsmith(__dirname)
        .use(dateInFilename({override: true}))
        .build();

... alternatively, you can pass just a boolean to the plugin, and the `override` setting will be set to it:

    ...
        .use(dateInFilename(true))
    ...


CLI Usage
----

    {
        "plugins": {
            "metalsmith-date-in-filename": {"override": true}
        }
    }


License
----

ISC

