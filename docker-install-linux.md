## Create a native Linux Environment

You can use ONE (1) of the follow two (2) options:

1. Use your laptop with a Linux Distro installed (Preferably Ubuntu as per our examples below)
OR
2. A Linux VM on Azure: Click this [link](https://portal.azure.com/?feature.customportal=false#create/Canonical.UbuntuServer1710-ARM) to create a Ubuntu VM in Azure

**Note:**
- For ease of creation, use Password authentication instead of SSH Key
- Password must be min of 12 characters with at least one Uppercase, one numeric or special character 
- Choose DS1V2 for Virtual machine size 
- Once the machine is deployed successfully, make a note of the virtual machine's Public IP address 

## Setup Docker on Ubunutu ( Video) 
**Check out the video on how to install Docker on Ubuntu :** [https://www.youtube.com/watch?v=V9AKvZZCWLc](https://www.youtube.com/watch?v=V9AKvZZCWLc)

For manual instructions of setting up Docker on Ubuntu see below ...

### Install Putty to access your VM (Windows Users Only!)

    Download putty.exe (https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html ) locally on your laptop to SSH into the virtual machine
    Open Putty.exe and enter the IP address in Host text field and click on Open
     
    You will see an alert, click on Yes 
     
    Login with the credentials you configured during Step 1 (Create a Linux Bash Shell) 

### Install Docker on the linux machine  

    # Run the following commands to set up Docker engine and CLI tools

    # Update your repository manager
    sudo apt-get update 

    # Install package dependencies
    sudo apt-get install apt-transport-https ca-certificates curl software-properties-common 
    curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - 

    # Add the docker gpg keys
    sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" 
     
    # Install Docker CE
    sudo apt-get update 
    sudo apt-get install docker-ce 
    
    # Verify Docker Installation 
    sudo docker run hello-world 
