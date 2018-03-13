## Create native Windows Environment

### Before you install Docker on Windows 

Requires Microsoft Windows 10 Professional or Enterprise 64-bit. Install [Docker Toolbox](https://docs.docker.com/toolbox/overview/) for older version of Windows 

Documentation : [Docker on Windows](https://store.docker.com/editions/community/docker-ce-desktop-windows)
### Setup Docker on Windows 10 (Video) 
**Check out the video on how to install docker on Windows**:[https://www.youtube.com/watch?v=S7NVloq0EBc](https://www.youtube.com/watch?v=S7NVloq0EBc)

For manual isntructions see below .... 

### Install
Double-click Docker for Windows Installer to run the installer. 

**[Get Docker CE for Windows](https://download.docker.com/win/stable/Docker%20for%20Windows%20Installer.exe)**

When the installation finishes, Docker starts automatically. The whale  in the notification area indicates that Docker is running, and accessible from a terminal.

### Run
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
