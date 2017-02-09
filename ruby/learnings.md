---
title: Static Analysis for Ruby
---

## Installing [SonarQube](http://www.sonarqube.org/)

Use [Homebrew](/tools/homebrew.html) to install SonarQube:

```bash
$ brew install sonarqube
$ brew tap homebrew/services
$ brew services start sonarqube
```

Then visit <http://localhost:9000/>

## Running with Maven

If you have a Maven project that you'd like to run against SonarQube, all you need to do is run the following:

```bash
$ mvn sonar:sonar
```

Then visit <http://localhost:9000/> and you should see your project listed.

## Running with Gradle

Open your project's `build.gradle` and add the following:

```groovy
apply plugin: 'sonar-runner'
```

Then run the following from the command-line:

```bash
$ gradle sonarRunner
```

Then visit <http://localhost:9000/> and you should see your project listed.
