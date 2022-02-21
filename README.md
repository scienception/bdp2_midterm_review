# bdp2_midterm_review

docker run -p 8888:8888 catecb/bdp2_midterm_review


### Run jupyter with persistance enabled (link host to container directory)

docker run -d --rm --name my_jupyter -v /home/enigma/review/work:/home/jovyan/work -p 8888:8888 --user root -e CHOWN_HOME=yes -e CHOWN_HOME_OPTS="-R" -e JUPYTER_TOKEN="bdp_password" catecb/bdp2_midterm_review

### Create an application stack with dockercompose

/usr/local/bin/docker-compose up -d

Make sure you're using latest docker-compose version

