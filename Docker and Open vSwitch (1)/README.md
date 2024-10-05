In this workshop, we will get introduced to Docker and Open vSwitch as the fundamental technologies for creating
virtual network topologies. Sections 2 and 3 provide relevant background and usage respectively of Docker and Open
vSwitch. 

1 Expected outcome
In this workshop, the student would learn about:
1. Using Docker as virtualization tool to create virtual hosts
2. Using Open vSwitch to create a virtual network topology
3. Connect the virtual hosts to virtual switches and test connectivity
This workshop and all subsequent ones need to be implemented on a Linux host. All workshops have been tested
on an Ubuntu 16.04 Virtual Machine on VirtualBox.


2 Background
This section provides a basic background about Docker and Open vSwitch.
2.1 Docker
Docker is essentially operating-system-level virtualization which allows developing and deploying software in packages
called containers. Docker containers are isolated from each other and bundle their own software, libraries and configu-
ration files - and therefore are platform independent. Containers use the kernel of the host machine, and are therefore
much more lightweight compared to virtual machines.
A container is deployed using an image that specifies the details of the container. An image is usually built by
extending a base image (e.g. ubuntu-trusty) with specific configurations.
Install Docker on the Linux host by following the instructions in the following link : How To Install and Use Docker
on Ubuntu 16.04 1.
Upon installing Docker, you need to start Docker service by using the following command.
$ sudo systemctl start docker
