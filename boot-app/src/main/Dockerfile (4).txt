FROM adoptopenjdk/openjdk11:alpine-jre

ARG artifact=target/java-web-app*.war

WORKDIR /opt/app

COPY ${artifact} app.war

ENTRYPOINT ["java","-jar","app.war"]
