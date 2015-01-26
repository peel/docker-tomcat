#Idea
The idea for the image is to create a lightweight Tomcat container that will automatically add any war file generated into target directory of your project.
The base image is Busybox w/ OpenJDK (Zulu VM).

#Tags
The repository contains several tags for various versions of Tomcat.
Pattern for tagging versions:

- 8, 8.0.17, latest - Tomcat 8.0.17
- 7, 7.0.57  - Tomcat 7.0.57

Older versions might be available under respectable version tags.

#Usage
As template:

```
FROM peelsky/tomcat:8
MAINTAINER Piotr Limanowski <plimanowski@gmail.com>
```

From command line:
```
docker run --rm -p 8080:8080 -it peelsky/tomcat:8
```
