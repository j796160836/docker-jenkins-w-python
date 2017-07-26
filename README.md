# Jenkins with Python

A Jenkins image with python environment.

- Python 2.7.13
- Openjdk 1.8.0_131
- Based on Alpine linux 3.6 Image

See `DockerFile` for details.

## Usage

### Run jenkins
```
$ docker run -idt -p 8080:8080 -v jenkins_home:/var/jenkins_home j796160836/jenkins-w-python:py2-jdk8
```
See offical document for further more details:  
[https://github.com/jenkinsci/docker](https://github.com/jenkinsci/docker)

#### Unlock Jenkins for setup
```
$ docker exec <container_id> cat /var/jenkins_home/secrets/initialAdminPassword
```

#### Run bash
```
$ docker exec -it <container_id> /bin/bash
```