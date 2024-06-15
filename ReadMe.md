Clean all docker cache by force

```bash
docker system prune -a --volumes --force ## delete all data
docker stop $(docker ps -a -q) ## stop all process
docker rm $(docker ps -a -q) ## remove all containers
```