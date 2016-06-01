# Manages Images and Containers.

# List All Containers 
docker ps -a

#Start Container using ContainerID:
docker start <ContainerID>

#Stop Container using ContainerID:
docker stop <ContainerID>

# Getting Terminal Access. This will start another process
sudo docker exec -i -t <ContainerID> bash

# Delete Containers
sudo docker rm <ContainerID or ContainerName>

# Delete Images by using Repository:tag or ImageID
sudo docker rmi <Repository>:<tag>
sudo docker rmi <ImageID>





