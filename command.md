 # command to see hidden files
 ls -lart
 # command to view all docker images
 docker images
 # command for freezing all libraries in use
 pip freeze >> <requirements.txt>
 # command to remove images
 docker rmi <imageid>
 # command to remove all images and containers
  docker system prune   
# To build docker image
# Mkae sure you have created your docker file
# Mkae sure your docker dexktop is up and running
# Get the list of docker images locally
 $ docker images
 $ docker images -a
# Comand to build your image
 docker build -t engrvic/flask-project .
# Apply force to delete 1st, 2nd, 3rd, 4th
 $ docker images purge
 $ docker images prune
 # powerful ones
 $ docker image prune --all --force
 $ docker rmi -f $(docker images -aq)
# To check the list of containers
 $ docker ps
# to create a container or build docker container
docker run -dp <5004:5004> <diamondimage> 
# to list container that is both running or not running 
docker ps -a
# To remove containers 
docker rm -vf $(docker ps -a -q)
# to stop a running container
docker stop containername
# To push your docker images to dockerhub
docker push engrvic/flask-project