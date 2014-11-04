metalsmith-date-in-filename: incorporate date info in filename onto file metadata.
====

[![Build Status](https://travis-ci.org/sanx/metalsmith-date-in-filename.svg?branch=master)](https://travis-ci.org/sanx/metalsmith-date-in-filename)

Installation
----

`npm install --save-dev metalsmith-date-in-filename`

Usage
----

    var Metalsmith = require('Metalsmith');
    var dateInFilename = require('metalsmith-date-in-filename');
    Metalsmith(__dirname)
        .use(dateInFilename({override: true})) // can be "dateInFilename(true)", which is equivalent
        .build();


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

