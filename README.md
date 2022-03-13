# Android-BuildSrc

## What is buildSrc?

buildSrc is a directory at the project root level which contains build info. 
We can use this directory to enable kotlin-dsl and write logic related to custom configuration and share them across the project. 
It was one of the most used approaches in recent days because of its testability,

_The directory buildSrc is treated as an included build. 
Upon discovery of the directory, Gradle automatically compiles and tests this code and puts it in the classpath of your build script. 
For multi-project builds there can be only one buildSrc directory, which has to sit in the root project directory. 
buildSrc should be preferred over script plugins as it is easier to maintain, refactor and test the code.
[Gradle Docs](https://docs.gradle.org/current/userguide/organizing_gradle_projects.html#sec:build_sources)_

## Reasons for using it:

* Avoid conflicting versions
* Better Management over depenecies.

## Steps to use:

* Copy [buildSrc](/buildSrc) folder into your project root folder.
* Sych the project.
* And you're ready to use this in your projects.
* for ref just look [demo](/buildSrc/demo_build.gradle.kts.txt)





