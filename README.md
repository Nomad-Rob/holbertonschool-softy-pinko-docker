Messing with Docker!!!!

Some useful commands:

- `docker build -t <name> .` - Builds a docker image from the Dockerfile in the current directory
- `docker run -it <name>` - Runs the docker image in a container
- `docker run -it -v <host_path>:<container_path> <name>` - Runs the docker image in a container with a volume mounted
- `docker run -it -p <host_port>:<container_port> <name>` - Runs the docker image in a container with a port mapped
- `docker run -it -p <host_port>:<container_port> -v <host_path>:<container_path> <name>` - Runs the docker image in a container with a port mapped and a volume mounted
- `docker run -it -p <host_port>:<container_port> -v <host_path>:<container_path> --name <container_name> <name>` - Runs the docker image in a container with a port mapped, a volume mounted, and a name
- `docker ps` - Lists all running containers
- `docker ps -a` - Lists all containers
- `docker stop <container_name>` - Stops a container
- `docker rm <container_name>` - Removes a container
- `docker rmi <name>` - Removes an image
- `docker exec -it <container_name> <command>` - Runs a command in a running container
- `docker exec -it <container_name> bash` - Runs a bash shell in a running container
- `docker exec -it <container_name> sh` - Runs a sh shell in a running container
- `docker exec -it <container_name> python` - Runs a python shell in a running container
- `docker exec -it <container_name> python <script>` - Runs a python script in a running container
- `docker exec -it <container_name> python3` - Runs a python3 shell in a running container
- `docker exec -it <container_name> python3 <script>` - Runs a python3 script in a running container
- `docker exec -it <container_name> ipython` - Runs an ipython shell in a running container
- `docker exec -it <container_name> ipython <script>` - Runs an ipython script in a running container
- `docker exec -it <container_name> ipython3` - Runs an ipython3 shell in a running container
- `docker exec -it <container_name> ipython3 <script>` - Runs an ipython3 script in a running container
- `docker exec -it <container_name> jupyter notebook --ip

Some commands I used to build this:

- docker build -f ./Dockerfile -t softy-pinko:task# . # Build the image
- docker run -it --rm --name softy-pinko-task0 softy-pinko:task# # Run the image
- docker-compose build # Build the image in the docker-compose.yml file
- docker-compose up # Run the image in the docker-compose.yml file
