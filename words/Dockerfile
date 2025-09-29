FROM ubuntu:latest
RUN apt-get update

RUN apt-get install -y maven openjdk-8-jdk
ADD src/main/java ./src/main/java 
ADD target ./target
ADD pom.xml ./pom.xml

RUN mvn verify
CMD ["java", "-Xmx8m", "-Xms8m", "-jar", "./target/words.jar"]
