this repo allows you to use docker via jenkins, with no permission error.
# STEPS TO START JENKINS ON A LINUX SERVER
- create a user on your host machine or use one `useradd -m jenkins-user`
- make the user is owner of docker on host machine `sudo chown jenkins-user:jenkins-user /var/run/docker.sock`
- switch to the user `su jenkins-user`  
- go to the home of jenkins-user `cd ~`
- clone this repo `git clone https://github.com/feyzullahyildiz/jenkins-manages-host-docker.git`
- go to the repo path `cd jenkins-manages-host-docker`
- create the jenkins volume folder `mkdir jenkins_home`
- start the compose file `docker-compose up`
- then it should start at port 8080.
