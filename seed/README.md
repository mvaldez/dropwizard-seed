# Dropwizard Seed Project

Base project for building a [Dropwizard](http://www.dropwizard.io) application.  Creates a fat jar using John Rengelman's [ShadowJar](https://github.com/johnrengelman/shadow) plugin.

## System Requirements

- Java 8+

### How to generate Intellij project files

    ./gradlew idea

### How to build the server (default) - produces a fat jar at build/libs/projectName-version-all.jar

    ./gradlew clean build shadowJar

### How to start a development server

    ./gradlew run

### Service Operations

    /person/get/{id} – by provided person unique “id” it returns JSON with person data
    /person/remove – removes one person on random basis
    /person/all – returns JSON with all persons data
    /person/save – receives JSON with person data and saves it to persons if “id” is unique, if not updating person by its id.
