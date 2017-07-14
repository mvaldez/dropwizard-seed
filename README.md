# Dropwizard Seed Project

This generates all the base projects files and directories for a Dropwizard application.  The build script utilizes Mitchell Bosecke's [Pebble](http://www.mitchellbosecke.com/pebble/home) template library.

The generated seed project is setup to work with both Gradle and Maven.

Project seed files/dirs scheme were generated using Maven.

	mvn -B archetype:generate
		-DarchetypeGroupId=org.apache.maven.archetypes
		-DgroupId=com.domain.projectName
		-DartifactId=MyApp

## How to create seed project

	Update gradle.properties. Spaces are not supported.

		projectName - project or application name e.g. com.domain.projectName
		dropwizardVersion - Dropwizard version this project will use
		domain - application domain name  e.g. com.domain.myapp
		artifactId - artifact identifier e.g. MyAwesomeApp

	Execute build script

		$ ./gradlew seed
	
	Distribution located at build/distributions/<projectName>

