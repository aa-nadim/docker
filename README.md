# Docker

```
Stop All Running Containers

docker stop $(docker ps -aq)
________________________________________________
Remove All Containers
docker rm $(docker ps -aq)
____________________________

Remove All Images
docker rmi $(docker images -q) --force
____________________________


Remove All Volumes
docker volume rm $(docker volume ls -q)
____________________________

Remove All Networks
docker network rm $(docker network ls -q)
____________________________

Remove All Docker Data
docker system prune --all --force
____________________________

Remove Docker Images
docker rmi -f $(docker images -a -q)
____________________________

Clean Up Docker System (Optional)
docker system prune -a --volumes
```