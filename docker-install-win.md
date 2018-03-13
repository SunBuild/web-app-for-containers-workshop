## Create native Windows Environment

### Before you install Docker on Windows 

**README FIRST for Docker Toolbox and Docker Machine users**: Docker for Windows requires Microsoft Hyper-V to run. The Docker for Windows installer enables Hyper-V for you, if needed, and restart your machine. After Hyper-V is enabled, VirtualBox no longer works, but any VirtualBox VM images remain. VirtualBox VMs created with docker-machine (including the default one typically created during Toolbox install) no longer start. These VMs cannot be used side-by-side with Docker for Windows. However, you can still use docker-machine to manage remote VMs. 

  
### Setup Docker on Windows 10 (Video) 
**Check out the video on how to install docker on Windows**:[https://www.youtube.com/watch?v=S7NVloq0EBc](https://www.youtube.com/watch?v=S7NVloq0EBc)

For manual isntructions see below .... 

### Install Docker Tool box 

Install [Docker Toolbox](https://docs.docker.com/toolbox/overview/), which uses Oracle Virtual Box instead of Hyper-V. 
What the Docker for Windows install includes: The installation provides Docker Engine, Docker CLI client, Docker Compose, Docker Machine, and Kitematic.

For  full documentation on installing Docker toolbox , click [here](https://docs.docker.com/toolbox/toolbox_install_windows/#step-2-install-docker-toolbox)

### Check if docker is installed 

Open Command prompt or Powershell in administrator mode and run the following commands to set up Docker engine and CLI tools

 ```
PS C:\Users\jdoe> docker --version
Docker version 17.03.0-ce, build 60ccb22

PS C:\Users\jdoe> docker run hello-world

Hello from Docker.
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
1. The Docker client contacted the Docker daemon.
2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
3. The Docker daemon created a new container from that image which runs the executable that produces the output you are currently reading.
4. The Docker daemon streamed that output to the Docker client, which sent it to your terminal.
```
