# Simple Docker

## Part1. Ready-made docker

1. Screenshot answers to these tasks enumerate below:

* Take the official docker image from nginx and download it using docker pull.
* Check for the docker image with docker images.
* Run docker image with docker run -d [image_id|repository].
* Check that the image is running with docker ps.
![1](./../images/Part1/1.png)

2. Screenshot answers to these tasks enumerate below:

* View container information with docker inspect [container_id|container_name].
* From the command output define and write in the report the container size, list of mapped ports and container ip.
* Stop docker image with docker stop [container_id|container_name].
* Check that the image has stopped with docker ps.
![2](./../images/Part1/2.png)

3. Screenshot answers to these tasks enumerate below:

* Run docker with ports 80 and 443 in container, mapped to the same ports on the local machine, with run command.
* Check that the nginx start page is available in the browser at localhost:80.
* Restart docker container with docker restart [container_id|container_name].
* Check in any way that the container is running.
Add the following screenshots to the report:
    the call and output of all commands used in this part of the task;
    nginx start page at localhost:80 (address must be shown).
![3](./../images/Part1/3.png)

## Part 2. Operations with container

1. Screenshot answers to these tasks enumerate below:

* Read the nginx.conf configuration file inside the docker container with the exec command.
![1](./../images/Part2/1.png)

2. Screenshot answers to these tasks enumerate below:

* Create a nginx.conf file on a local machine.
* Configure it on the /status path to return the nginx server status page.
![2](./../images/Part2/2.png)

3. Screenshot answers to these tasks enumerate below:

* Copy the created nginx.conf file inside the docker image using the docker cp command.
* Restart nginx inside the docker image with exec.
* Check that localhost:80/status returns the nginx server status page.
![3](./../images/Part2/3.png)

4. Screenshot answers to these tasks enumerate below:

* Export the container to a container.tar file with the export command.
* Stop the container.
* Delete the image with docker rmi [image_id|repository]without removing the container first.
* Delete stopped container.
![4](./../images/Part2/4.png)

5. Screenshot answers to these tasks enumerate below:

* Import the container back using the importcommand.
* Run the imported container.
* Check that localhost:80/status returns the nginx server status page.
![5](./../images/Part2/5.png)