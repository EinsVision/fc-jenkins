# jenkins
# This is for the Jenkins project

    * Jenkins docker 20260915 installed
      docker run -d --name jenkins --hostname=jenkins \
                 --restart=on-failure \
                 -e TZ=Europe/Berlin \
                 -p 8082:8080 -p 50000:50000 \
                 -v ${HOME}/practice/key:/key \
                 -v ${HOME}/.jenkins:/var/jenkins_home \
                 -v /var/run/docker.sock:/var/run/docker.sock \
                 --network practice \
                 --user root \
                 jenkins/jenkins:latest-jdk21


## Test md file
