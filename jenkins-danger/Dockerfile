FROM jenkins

USER root
RUN apt-get update && apt-get install -y ruby make
RUN gem install danger
RUN mkdir -p /home/jenkins/danger