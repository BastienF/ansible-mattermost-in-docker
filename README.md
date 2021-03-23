# ansible-mattermost-in-docker

Build team app :
```
cd /tmp/
git clone git@github.com:mattermost/mattermost-docker.git
cd mattermost-docker/app/
git checkout v5.31.1
docker build . --build-arg edition=team -t bastienf/mattermost-app:v5.31.1
docker push bastienf/mattermost-app:v5.31.1
```