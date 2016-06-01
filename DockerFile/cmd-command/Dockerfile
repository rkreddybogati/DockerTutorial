# Installing applications in ubuntu base image.

FROM ubuntu:14.04

RUN apt-get update && apt-get install -y \
	curl \
	vim \
	openjdk-7-jdk

CMD ["ping", "127.0.0.1", "-c", "30"]  
 
