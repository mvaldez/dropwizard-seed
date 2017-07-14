# Dropwizard Seed Project

Base project for building a [Dropwizard](http://www.dropwizard.io) application.  Creates a fat jar using John Rengelman's [ShadowJar](https://github.com/johnrengelman/shadow) plugin.

## System Requirements

- Java 8+

### How to generate Intellij project files

	./gradlew idea

### How to build the server (default) - produces a fat jar at build/libs (projectName-all.jar)

	./gradlew clean build shadowJar

### How to start a development server

	./gradlew run
