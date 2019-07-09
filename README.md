# maven-archetype-swagger

A custom Maven archetype for creating multi-module project that can be used as a skeleton with [swagger-codegen-templates](https://github.com/mkatircioglu/swagger-codegen-templates). 

## Requirements

- Java 1.8
  - **because this archetype uses a post-generate Groovy script it doesn’t work on Java 9+**
- Maven 3.5

## Usage

To create a new project from this archetype, type:

```java
mvn archetype:generate \
-DarchetypeGroupId=io.github.mkatircioglu \
-DarchetypeArtifactId=maven-archetype-swagger \
-DarchetypeVersion=1.0.0-RELEASE
```
When prompted, enter the archetype properties for creating a new project.

You may find it easier to specify the archetype properties on the command line rather than interactively:

```java
mvn archetype:generate \
-DarchetypeGroupId=io.github.mkatircioglu \
-DarchetypeArtifactId=maven-archetype-swagger \
-DarchetypeVersion=1.0.0-RELEASE \
-DgroupId=com.samples \
-DartifactId=todo \
-Dversion=1.0.0-SNAPSHOT \
-Dpackage=com.samples.todo \
-Dspring-boot-starter-version=2.1.5.RELEASE \
-Dswagger-codegen-templates-version=1.0.0-RELEASE \
-Dswagger-maven-plugin=2.3.1

```

## License

This software is licensed under the terms in the file named “LICENSE” in the root directory of this project.

## Author

Mete Alpaslan KATIRCIOGLU <mete[at]katircioglu.net>