FROM adoptopenjdk/openjdk11:alpine-jre

ARG artifact=target/boot-web.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

ENTRYPOINT ["java","-jar","app.jar"]
