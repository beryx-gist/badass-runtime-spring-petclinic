[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/beryx-gist/badass-runtime-spring-petclinic/blob/master/LICENSE)
[![Build Status](https://img.shields.io/travis/beryx-gist/badass-runtime-spring-petclinic/master.svg?label=Build)](https://travis-ci.org/beryx-gist/badass-runtime-spring-petclinic)

## Custom runtime image of spring-petclinic using the badass-runtime plugin ##

This project demonstrates the capabilities of the [Badass Runtime Plugin](https://github.com/beryx/badass-runtime-plugin/)
by creating a custom runtime image of the [Spring PetClinic](https://github.com/spring-projects/spring-petclinic).

### Quick start
From the [releases page](https://github.com/beryx-gist/badass-runtime-spring-petclinic/releases) download the archived custom runtime image for your operating system.
Unpack the archive and execute the `spring-petclinic` script found in the `spring-petclinic-image/bin` directory.  
Then, access http://localhost:8080/ in your browser.

### Creating a custom runtime image

Gradle must use Java 11 in order to be able to build the project.
To create the custom runtime image execute:

```
./gradlew runtimeZip
```

This command creates the runtime image in the `build/spring-petclinic-image` directory and a zip file of it in `build/image-zip`.

The start scripts are found in the `build/spring-petclinic-image/bin` directory.
