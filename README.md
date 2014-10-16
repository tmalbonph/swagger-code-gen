## A client/server/database code generator from a Swagger 2.0 Specification file

swagger-code-gen
================

A code generator project.

### What is swagger-code-gen?

This software is a [NodeJS](http://nodejs.org) application.

It is intended for generating [Client side](https://github.com/tmalbonph/swagger-clent-gen), [Server side](https://github.com/tmalbonph/swagger-server-gen) and [Server database](https://github.com/tmalbonph/swagger-dbf-gen) [NodeJS](http://nodejs.org) codes from a Swagger Specification file in [version 2.0](https://github.com/reverb/swagger-spec/blob/master/versions/2.0.md) document format.

It is design to be run with [npm](https://www.npmjs.org/package/npm) using `npm run-script {XXXX};` where XXXX is one of demo, gen, test.

### How to install

* install [grunt-cli](https://github.com/gruntjs/grunt)

 `npm install -g grunt-cli`

* install its dependencies

 `npm install`

### How to create the provided sample demo

* create ``Sari-Sari store`` demo with npm

 `npm demo`

* create ``Sari-Sari store`` demo with node

 `node demo.js`

### How to generate code from your swagger 2.0 file

* generate with npm

 `npm run-script gen -c PATH/TO/YOUR/CONFIG/FILE -m [development staging qc production]`

* generate with node

 `node gen.js -c PATH/TO/YOUR/CONFIG/FILE -m [development staging qc production]`

* the configuration in JSON format should content information like
 ```
        {
        "development" : {
        "swaggerSpec" : "PATH/TO/SWAGGER/FILE",
        "gen" : {
            "dbf" : false,
            "client" : true,
            "server: false
        },
        "path" : {
            "dbf" : "PATH/TO/DATABASE/FOLDER",
            "client" : "PATH/TO/CLIENT/FOLDER",
            "server: "PATH/TO/SERVER/FOLDER"
        },
        "sql" : {
            "server" : "postgres",
            "user" : "USERNAME",
            "password" : "PASSWORD",
            "database" : "DATABASE-NAME",
            "connectionstring" : "CONNECTION-STRING"
        }
        },
        "staging" : {
        },
        "qc" : {
        },
        "production" : {
        },
        }
 ```
### Sample codes

* TODO : soon will add code snippets here

### License

[MIT](https://github.com/tmalbonph/swagger-code-gen/blob/master/LICENSE)

The MIT License (MIT)

Copyright (c) 2014 tmalbonph <tmalbonph@yahoo.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

### Current status

The current version of this software is under development and working in local repository. Will soon publish beta version.

