FROM amazonlinux:latest
RUN echo 'proxy=http://proxy-aws.risorse.enel:8080' >> /etc/yum.conf
RUN yum -y install java-1.8.0
EXPOSE 8080
ADD HelloWorld-1.0.jar HelloWorld-1.0.jar
ENTRYPOINT ["java","-jar","HelloWorld-1.0.jar"]