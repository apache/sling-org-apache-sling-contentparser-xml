[<img src="https://sling.apache.org/res/logos/sling.png"/>](https://sling.apache.org)

 [![Build Status](https://builds.apache.org/buildStatus/icon?job=Sling/sling-org-apache-sling-contentparser-xml/master)](https://builds.apache.org/job/Sling/job/sling-org-apache-sling-contentparser-xml/job/master) [![Test Status](https://img.shields.io/jenkins/t/https/builds.apache.org/job/Sling/job/sling-org-apache-sling-contentparser-xml/job/master.svg)](https://builds.apache.org/job/Sling/job/sling-org-apache-sling-contentparser-xml/job/master/test_results_analyzer/) [![Maven Central](https://maven-badges.herokuapp.com/maven-central/org.apache.sling/org.apache.sling.contentparser.xml/badge.svg)](https://search.maven.org/#search%7Cga%7C1%7Cg%3A%22org.apache.sling%22%20a%3A%22org.apache.sling.contentparser.xml%22) [![JavaDocs](https://www.javadoc.io/badge/org.apache.sling/org.apache.sling.contentparser.xml.svg)](https://www.javadoc.io/doc/org.apache.sling/org.apache.sling.contentparser.xml) [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0) [![contentparser](https://sling.apache.org/badges/group-contentparser.svg)](https://github.com/apache/sling-aggregator/blob/master/docs/groups/contentparser.md)

Apache Sling Content Parser for XML
====
This module is part of the [Apache Sling](https://sling.apache.org) project.

The Apache Sling Content Parser for XML provides support for parsing XML files into Apache Sling resource trees, by implementing the 
API provided by the [`org.apache.sling.contentparser.api`](https://github.com/apache/sling-org-apache-sling-contentparser-api) bundle.

To obtain a reference to the XML content parser just filter on the `ContentParser.SERVICE_PROPERTY_CONTENT_TYPE` service registration 
property:

```java
    @Reference(target = "(" + ContentParser.SERVICE_PROPERTY_CONTENT_TYPE + "=xml)")
    private ContentParser xmlParser;
``` 
