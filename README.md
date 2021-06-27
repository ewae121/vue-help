# Docker help

Memo on what was interesting things about VueJs

## Remove all images

```
docker kill $(docker ps -q)
docker rm $(docker ps -a -q)
docker rmi $(docker images -q)
docker rmi -f$(docker images -q)
docker rmi -f $(docker images -q)
```

## Move docker /var/lib

### Stop docker

```
sudo service docker stop
```

### Update docker configuration

__I place it to /home/docker often or a separate partition__

Add a file /etc/docker/daemon.json containing

```
{ 
   "data-root": "/path/to/your/docker" 
}
```

### Copy data to the new folder

```
sudo rsync -aP /var/lib/docker/ /path/to/your/docker
```

### Save the data

```
sudo mv /var/lib/docker /var/lib/docker.old
```

### Restart the service

```
sudo service docker start
```

### Test

Test it and if everything works fine. You can remove the folder.

```
sudo rm -rf /var/lib/docker.old
```
