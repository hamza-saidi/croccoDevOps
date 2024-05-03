FROM openjdk:8
EXPOSE 8089
WORKDIR /app

ADD http://0.0.0.0:8081/repository/maven-releases/tn/esprit/spring/gestion-station-ski/1.0/gestion-station-ski-1.0.jar gestion-station-ski-1.0.jar


ENTRYPOINT ["java", "-jar", "gestion-station-ski-1.0.0.jar"]
