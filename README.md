# weaveDemo
Demo microservices application for Weave.


# Installing
## Local
```
./scripts/install.sh launch
./build.sh
eval $(docker-machine env --swarm swarm-master)
docker-compose pull
docker-compose build
docker-compose up -d
```
Swarm up's are unstable. Pulling and building the project in stages seems to be more stable.

# Uninstalling
This will remove all docker-machines.
```
./scripts/install.sh destroy
```