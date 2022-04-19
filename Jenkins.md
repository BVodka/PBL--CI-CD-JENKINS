# Documentation for Project 9 - Automation with Jenkins
- Step 1 -- Setup Servers on AWS 
  
   - `sudo apt-get update && sudo apt-get upgrade` 
   - `sudo nano shell.sh && sudo chmod +x shell.sh`
  
### Bash Script to setup Jenkins

    ```
    #!/bin/bash
    sudo apt update -y
    sudo apt install default-jdk-headless -y

    wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
    sudo sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > \
    /etc/apt/sources.list.d/jenkins.list'
    sudo apt update -y
    sudo apt-get install jenkins -y 
    ```

### Run bash script 

    `sudo su  && ./shell.sh`

   -  ![Connecting to the EC2-instance and Setup Jenkins](./images/Capture_ConnectEC2_SetUp_Jenkins_Step1&2.JPG)
  
   -  ![Capture Jenkins Running](./images/Capture_Jenkins_Running_Step3.JPG)

### Setting Up Jenkins 

   -  ![Login to Jenkins](./images/Capture_LoginJenkins_Step4.JPG)
  
   -  ![Install Jenkins Plugins and Create User](./images/Capture_InstallPlugins_CreateAdminUser_Step5.JPG)
  
   -  ![Configure Jenkins Credentials](./images/Capture_Configure_Credentials_Jenkins_Step6.JPG)

## Builds 

   -  ![Local build console output](./images/Capture_ConsoleOutputBuild_Step7.JPG)
  
   -  ![Build from Github](./images/images\Capture_BuildfromGithub_Step8.JPG)
  
   -  ![Github Console Output](./images/Capture_ConsoleOutputGithub_Step9.JPG)
  
   -  ![Local Builds](./images/Capture_LocalBuilds_Step10.JPG)
  
### Configure Build from Github

   -  ![Configure SSH Plugin](./images/Capture_Configure_SSH_Plugin_Step11.JPG)
  
   -  ![SSH Build Error](./images/images/Capture_BuildErrorSSHTransfer_Step12.JPG)
  
   -  ![Change Permissions to folder /mnt/apps ](./images/Capture_ChangePermission_mntapps_Step13.JPG)
  
   -  ![SSH build successful](./images/Capture_SSH_Transfer_ConsoleSuccess_Step14.JPG)
  
   -  ![NFS Server](./images/Capture_NFS_Server_Step16.JPG)
  
