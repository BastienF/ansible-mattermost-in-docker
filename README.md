# ansible-mattermost-in-docker

Build team app :
```
cd /tmp/
git clone git@github.com:mattermost/mattermost-docker.git
cd mattermost-docker/app/
git checkout 5.12.1
docker build . --build-arg edition=team -t bastienf/mattermost-app:5.12.1
docker push bastienf/mattermost-app:5.12.1
```