 # command to see hidden files
 ls -lart
 # command to view all docker images
 docker images
 # command for freezing all libraries in use
 pip freeze >> <requirements.txt>
 # command to remove images
 docker rmi <imageid>
 # command to remove all images
  docker system prune
  ls -lart   
# To build docker image
# Mkae sure you have created your docker file
# Mkae sure your docker dexktop is up and running
# Get the list of docker images locally
 $ docker images
 $ docker images -a
# Comand to build your image
 docker build -t eunicmage 
# Apply force to delete 1st, 2nd, 3rd, 4th
 $ docker images purge
 $ docker images prune
 # powerful ones
 $ docker image prune --all --force
 $ docker rmi -f $(docker images -aq)
# To build docker container image
 To build docker container image
 $ docker run -dp 5004:5004 eunicmage
 $ bb0b75a1d3161ed96649fe7cf1b83b0a047def89b1c24892583913a46a2a34f6

# To check the list of containers
 $ docker ps

# To remove unused all images and containers
docker system prune
# to create a container
docker run -dp <5004:5004> <diamondimage> 
# to list container 
docker ps
# To remove containers 
docker rm -vf $(docker ps -a -q)
# 