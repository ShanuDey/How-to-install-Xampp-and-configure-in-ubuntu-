# How-to-install-Xampp-and-configure-in-ubuntu-
How to install Xampp and configure in ubuntu?

# Installation
1) Download xampp from official website.
2) Run the file as root (Example: "sudo ./xampp-linux-x64-7.3.0-0-installer.run")
3) Follow the installation wizard (Next>NExt>Finish)
4) Wait until complete
5) It will install in /opt/lampp/
6) Open Terminal and Type : "sudo ./opt/lampp/manager-linux-x64.run"
7) Start all services
8) Test in browser. Visit : http://localhost

# Terminal commands
1) Starting xampp -> "sudo /opt/lampp/xampp start"
2) Stoping xampp -> "sudo /opt/lampp/xampp stop"
3) Status of services -> "sudo /opt/lampp/xampp status"
4) You may also use "sudo ./opt/lampp/lampp start". (Note lamp=>/opt/lampp/xapp)

# Configure 
1) Change htdocs folder is not permissible we need sudo everytime.
2) "sudo chmod 777 -R /opt/lampp/htdocs" works but it has security issue.(Google it)
3) Add this folder to your user:group
4) Type: "sudo chown -R username:groupname /opt/lampp/htdocs"
5) Change the permission to read, write execute. Type: "sudo chmod 700 /opt/lampp/htdocs"
6) You are ready to go

# Issue Fixing
1) May be your browser is unable to read htdocs.
2) And http://localhost give an error that no read and execute permission.
3) Solution is easy give the read and execute permission 
4) Don't give write permission to other it may cause security issue.
5) Type: "sudo chmod 755 -R /opt/lampp/htdocs"

## Enjoy your xampp

### Note
1) For more information about chmod type : man chmod or Google it

#### chmod XYZ -R /opt/lampp/htdocs
1)  X-> User permission
2)  Y-> Group permission
3)  Z-> Others permission
4)  -R (Recussively) flag is used to give this pemission all the subdirectory of that directory.
  
  ## Hope you enjoyed. Put a start on this repo. Thank you. 
  
