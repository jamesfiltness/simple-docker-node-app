docker build -t some-tag .
docker images --filter reference=some-tag
docker run -i -t -p 46190:80 some-tag

runs the docker container on port 46190

Currently Ctrl+c does not kill the container. Suggested solutions online do not seem to work. 
Currently using docker ps and docker kill pid to get around this.
