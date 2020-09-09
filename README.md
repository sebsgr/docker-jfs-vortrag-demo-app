# docker-jfs-vortrag-demo-app
Demo Projekt zum Vortrag "Just Docker" auf dem Java Forum Stuttgart 2020

### JAR erstellen - wird im Ordner build/libs abgelegt.

`.\gradlew bootjar`

### JARDockerfile und Jar in den Ordner build/docker kopieren.

`.\gradlew prepareForDockerBuild`

### JARDocker Image mit dem Tag docker-demo:latest erstellen.

`docker build -t docker-demo:latest build/docker/`

### JARDocker Container starten.

`docker run -it --rm -p 6080:8080 docker-demo:latest`
