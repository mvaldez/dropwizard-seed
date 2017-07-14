# Dropwizard Seed Project

Base project for building a [Dropwizard](http://www.dropwizard.io) application.  Creates a fat jar using John Rengelman's [ShadowJar](https://github.com/johnrengelman/shadow) plugin.

## Versions

    - java 8+
    - dropwizard-core 1.1.2
    - swagger-api 1.5.15
    - swagger-ui 2.2.10
    - gradle 3.1.0

## How to generate Intellij project files

    ./gradlew idea

## How to build the server (default)

Produces a fat jar at build/libs/projectName-version-all.jar

    ./gradlew clean build shadowJar

## How to start a development server

    ./gradlew run

## Sample Service Operations

    /person/get/{id} – by provided person unique “id” it returns JSON with person data
    /person/remove – removes one person on random basis
    /person/all – returns JSON with all persons data
    /person/save – receives JSON with person data and saves it to persons if “id” is unique, if not updating person by its id.
    /swagger - swagger UI

## Acknowlegdements

* Federico Recio [@federecio](http://twitter.com/federecio)
* Smoke Turner [smoketurner](https://github.com/smoketurner)
* Mike Lynch [nycnik](https://github.com/nycynik)
* John Rengelman [ShadowJar](https://github.com/johnrengelman/shadow)