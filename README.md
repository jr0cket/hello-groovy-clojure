# hello-gradle

A Clojure application to discover how to build this project using Gradle

## Usage

[Install Gradle](https://gradle.org/install/) 4.2.1 or greater.

The following commands have been tested and create the expected results.  

* `gradle clean`
* `gradle build`
* `gradle clojureTest`

Clean removes any Gradle generated assets (although not the Leiningen ones as it uses target rather than build directory).

The `build` task compiles the project and places the output in the build directory

The `clojureTest` task runs the clojure.test defined tests and outputs the results in XML format for the TeamCity server in the build/test-results directory.  The results of `clojureTest` are also shown on screen when run locally.


* `gradle uberjar`

The `uberjar` task seems to do everything except set the class name in the `META-INF/manifest` file.


To see all the task you can run for Gradle, then use the command:

`gradle tasks`

## License

Copyright © 2017 @jr0cket

Distributed under the Creative Commons Attribution Share-alike International 4.0 license
