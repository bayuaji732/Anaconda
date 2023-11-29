Anaconda Installation Guide for Multi user
Operating System
CentOS 7

Anaconda Installation Path
/opt/anaconda3

Step-by-Step Installation Guide
Create Anaconda Group:

bash
Copy code
sudo groupadd anaconda
Set Group Ownership to Anaconda:

bash
Copy code
sudo chgrp -R anaconda /opt/anaconda3
Set Permissions for Anaconda Directory:

bash
Copy code
sudo chmod 770 -R /opt/anaconda3
Add User to Anaconda Group:

bash
Copy code
sudo usermod -a -G anaconda <username>
Note:
Ensure that the Anaconda installation directory is /opt/anaconda3.
Replace <username> with the actual username you want to add to the Anaconda group.
