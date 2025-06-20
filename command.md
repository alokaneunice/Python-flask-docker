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

# To check the list of running containers
 $ docker ps
# to create a container or build docker container
docker run --name flask-container -dp 8081:8081 engrvic/flask-image
# to list container that is both running or not running 
docker ps -a
# to stop a running container
docker stop containername
# To push your docker images to dockerhub
docker push engrvic/flask-project
# to remove all docker images
docker rmi -f $(docker images -aq)
# To remove all docker containers
docker rm -vf $(docker ps -a -q)
# to get the content of a file
cat requirements.txt