# CICD-Ansible
CICD 파이프라인 고도화 연습

jenkins
docker images
docker ps
docker exec -it 66201609159c /bin/bash
docker run -d -v jenkins_home:/var/jenkins_home -p 8080:8080 -p 50000:50000 --restart=on-failure jenkins/jenkins:lts-jdk17

ansible
docker run --privileged --name ansible-server -itd -p 20022:22 -p 8081:8081 -e container=docker -v /sys/fs/cgroup:/sys/fs/ctroup edowon0623/ansible:latest /usr/sbin/init
