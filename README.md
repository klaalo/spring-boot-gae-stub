# Spring Boot App Engine Archetype

This is a simple archetype for creating a stub project
of [Spring Boot](https://projects.spring.io/spring-boot/)
to be run in [Google App Engine](https://cloud.google.com/appengine/).

Now that [Java 8](https://cloud.google.com/appengine/docs/standard/java/runtime-java8)
Runtime Environment [became supported](https://cloudplatform.googleblog.com/2017/06/Google-App-Engine-standard-now-supports-Java-8.html)
on app engine it makes convenient platform to run also Spring Boot applications.

Container environment, e.g. [Kubernetes](https://cloud.google.com/kubernetes-engine/),
would also make a great platform for Spring Boot. However, with app engine, you get
24 hours of free of charge instance hours. With Kubernetes you will pay for every
instance hour and the requirement of master node makes you pay fot at least for
two instances. So that maks app engine an inexpensive choice for trying out different
ideas.

## Usage

After cloning the project, install the archetype to your local repository

    cd spring-boot-gae-stub
    mvn install
    
Use archetype to create a new project stub

    mvn archetype:generate \
      -DarchetypeGroupId=fi.karilaalo \
      -DarchetypeArtifactId=spring-boot-gae-stub \
      -DarchetypeVersion=1.0-SNAPSHOT \
      -DgroupId=<groupId> \
      -DartifactId=<artifactId> \
      -Dversion=0-0-1-snapshot
      
Run stub project with dev server

	cd <artifactId>
    mvn appengine:run

## Credits

- https://github.com/GoogleCloudPlatform/getting-started-java/tree/master/appengine-standard-java8/springboot-appengine-standard
- https://codelabs.developers.google.com/codelabs/cloud-app-engine-springboot/index.html
- https://github.com/michaeltecourt/appengine-spring-boot