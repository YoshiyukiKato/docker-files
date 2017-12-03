FROM jenkins

USER root
ARG DANGER_GITHUB_API_TOKEN
ENV DANGER_GITHUB_API_TOKEN $DANGER_GITHUB_API_TOKEN
RUN apt-get update && apt-get install -y ruby make
RUN gem install bundler
USER jenkins