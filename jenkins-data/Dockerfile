FROM debian:jessie
MAINTAINER Ahmed Kamel

#Create jenkins user in this container
RUN useradd -d "/var/jenkins_home" -u 1000 -m -s /bin/bash jenkins

# Create Jenkins log dir
RUN mkdir -p /var/log/jenkins
RUN chown -R jenkins:jenkins /var/log/jenkins

# Create a docker mount
VOLUME ["/var/log/jenkins", "/var/jenkins_home"]

#Switch user to jenkins
USER jenkins

CMD ["echo", "Data container for Jenkins"]
