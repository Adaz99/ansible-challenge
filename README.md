Setup a virtual machine using Vagrant and link it to a shared folder (vm-share) that contains the "Jenkins Config" and "Inventory.txt" files.
Establish two AWS instances, one for the JenkinsHost and another for the agent, both running and working as seen in the recording below.
Access the Vagrant machine using SSH and transfer the shared folder to the Agent using the rsync command and the Ubuntu IP.


![demo](./Recording%202023-01-31%20at%2016.52.27.gif)