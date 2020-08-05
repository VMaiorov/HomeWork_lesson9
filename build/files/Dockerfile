FROM ubuntu:18.04
RUN apt update && \
    apt install -y default-jdk maven git && \
    export JAVA_HOME=/usr/lib/jvm/java-11-openjdk-amd64 && \
    export PATH=$PATH:$JAVA_HOME/bin && \
    git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
CMD mvn package -f /boxfuse-sample-java-war-hello/pom.xml  
