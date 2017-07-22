# Dropwizard/MongoDB Java Seed Project

This generates all the base projects files and directories for a Dropwizard application with MongoDB support.  The build script utilizes Mitchell Bosecke's [Pebble](http://www.mitchellbosecke.com/pebble/home) template library.

The generated seed project is setup to work with both Gradle and Maven.

Project seed files/dirs scheme were generated using Maven.

    mvn -B archetype:generate
        -DarchetypeGroupId=org.apache.maven.archetypes
        -DgroupId=com.domain.projectName
        -DartifactId=MyApp

## Versions

    - java 8+
    - dropwizard-core 1.1.2
    - swagger-api 1.5.15
    - swagger-ui 2.2.10
    - gradle 3.1.0

## How to create seed project

Update gradle.properties. Spaces are not supported.

    projectName - project or application name e.g. com.domain.projectName
    version - seed project's initial version
    domain - application domain name  e.g. com.domain.myapp
    subDomain - application sub domain e.g. subdomain.domain.myapp

Execute build script

    $ ./gradlew seed

Distribution location

    dropwizard-seed/build/distributions/<projectName>

## Acknowledgements

* Federico Recio [@federecio](http://twitter.com/federecio)
* Smoke Turner [smoketurner](https://github.com/smoketurner)
* Mitchell Bosecke [Pebble](http://www.mitchellbosecke.com/pebble/home) template engine support
* John Rengelman [ShadowJar](https://github.com/johnrengelman/shadow)
* Mike Lynch [nycnik](https://github.com/nycynik)
* Morphia [morphia](http://mongodb.github.io/morphia)
* MongoDB Java Driver [mongodb](https://mongodb.github.io/mongo-java-driver)
