FROM openjdk:8-jre
MAINTAINER Maria Pereira

ENTRYPOINT ["/usr/bin/java", "-jar", "/usr/share/myservice/myservice.jar"]

# Add Maven dependencies (not shaded into the artifact; Docker-cached)
ADD target         /usr/share/myservice/lib
# Add the service itself
ADD target/JavaProject-1.0-SNAPSHOT.jar /usr/share/myservice/myservice.jar