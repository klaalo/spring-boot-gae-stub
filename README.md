# Spring Boot App Engine Archetype

This is a simple archetype for creating a stub project
of [Spring Boot](https://projects.spring.io/spring-boot/)
to be run in [Google App Engine](https://cloud.google.com/appengine/).

## Usage

After cloning the project, install the archetype to your local repository.

    cd spring-boot-gae-stub
    mvn install
    
Use archetype to create a new project stub.

    mvn archetype:generate \
      -DarchetypeGroupId=fi.karilaalo \
      -DarchetypeArtifactId=spring-boot-gae-stub \
      -DarchetypeVersion=1.0-SNAPSHOT \
      -DgroupId=<groupId> \
      -DartifactId=<artifactId> \
      -Dversion=0-0-1-snapshot

## Credits

- https://github.com/GoogleCloudPlatform/getting-started-java/tree/master/appengine-standard-java8/springboot-appengine-standard
- https://codelabs.developers.google.com/codelabs/cloud-app-engine-springboot/index.html
- https://github.com/michaeltecourt/appengine-spring-boot