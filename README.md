# Devoxx workshop

## Prerequisite

- Download [ZAP](https://github.com/zaproxy/zaproxy/wiki/Downloads) and install it on your machine.
- Download [WebGoat v8.0.0.M21](https://github.com/WebGoat/WebGoat/releases/tag/v8.0.0.M21)
- Download [Java 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) only download, see below.
- Docker (optional)

You should be able to change the proxy settings of your laptop, if not please download Firefox Portable Edition (https://portableapps.com/apps/internet/firefox_portable)

If the internet connection is fast enough we will use the online version hosted on Google Cloud.

## Online

Open up a browser and point it to: http://1.1.1.1:8080/WebGoat/

Register as a new user.

## Run on local machine

**NOTE**: Only necessary if the online version is not available. Choose one of the options below:

### Running jar file

**Prerequisite: Java 8 should be present on laptop**

Start WebGoat:

```
java -jar webgoat-8.0.0-M21.jar
```

Using Java 9 or above, see https://github.com/WebGoat/WebGoat/wiki/FAQ#java9 for more information.

### Using Docker image from Docker Hub

**Prerequisite: Docker should be present on laptop**

```
docker run -p 8080:8080 -t webgoat/webgoat-8.0.0-M21
```
