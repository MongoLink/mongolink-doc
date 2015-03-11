# Mongolink 

Mongolink is an object/document mapper for java and MongoDB. 
More informations can be found [here](http://mongolink.org)

## Purpose

We wanted to build a persistence tool that achieves several key features:

 * Persistence ignorance : our domain should not depend on abstractions coming from the persistence mechanism. Yes, an annotation on a an object is such a coupling
 * We don't want to use annotations, yet we don't want either to maintain tons of xml files 
 * Domain Driven Design is cool stuff, we wan't our persistence tool to understands concepts as aggregates, value objects, and entities
 * Concurrency with mongodb can be tricky. Updating the whole document when it's changed is clearly not a good strategy

## Adding mongolink to your project

### Configuration for maven

```xml
<dependency>
  <groupId>org.mongolink</groupId>
  <artifactId>mongolink</groupId>
    <version>1.2.1</version>
</dependency>
```
### Configuration for gradle

```groovy
compile "org.mongolink:mongolink:1.2.1"
```

Next : [configuring Mongolink](configuration.md)