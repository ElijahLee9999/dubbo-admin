FROM java:8
LABEL maintainer elijah <workforelijah@hostmail.com>
WORKDIR /usr/local
ADD ../dubbo-admin-server/target/dubbo-admin-server-0.2.0-SNAPSHOT.jar .

EXPOSE 8080

ENTRYPOINT ["java","-XX:+UnlockExperimentalVMOptions","-XX:+UseCGroupMemoryLimitForHeap","-Djava.security.egd=file:/dev/./urandom","-jar","dubbo-admin-server-0.2.0-SNAPSHOT.jar"]
#ENTRYPOINT ["nohup","java","-jar","/usr/local/dubbo-admin-server-0.2.0-SNAPSHOT.jar",">","/usr/local/logs","2>&1","&"]