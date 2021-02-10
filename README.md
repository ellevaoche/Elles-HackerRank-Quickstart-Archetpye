# Elles HackerRank Quickstart Archetpye

## Summary

The project contains a customized Maven archetype (Java8, Junit5) which I use as template for new Java projects for [HackerRank.com](https://hackerrank.com) challenges.

- Some info about Maven Archetypes could be found here: <https://maven.apache.org/guides/introduction/introduction-to-archetypes.html>
- Helpful was also the following Tutorial: <https://www.baeldung.com/maven-archetype>

## Installation

To install the archetype in your local maven repository execute the following commands:

```bash
    git clone https://github.com/ellevaoche/Elles-HackerRank-Quickstart-Archetpye.git
    cd hackerrank-quickstart-archetype
    mvn clean install
```

## Create a project based on my Archetype

To generate a project from the custom archetype use one of the following methods:

### Interactive mode

```bash
mvn archetype:generate \
    -DarchetypeGroupId=com.hackerrank \
    -DarchetypeArtifactId=elle-hackerrank-quickstart-archetype \
    -DarchetypeVersion=1.0.0-SNAPSHOT \
```

### Non-Interactive mode

```bash
mvn archetype:generate \
    -DinteractiveMode=false \
    -DarchetypeGroupId=com.hackerrank \
    -DarchetypeArtifactId=elle-hackerrank-quickstart-archetype \
    -DarchetypeVersion=1.0.0-SNAPSHOT \
    -DgroupId=[myCustom.groupid] \
    -DartifactId=[myCustomArtifactId] \
    -Dversion=[myCustomVersion]
```
