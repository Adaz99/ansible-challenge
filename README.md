Setup a virtual machine using Vagrant and link it to a shared folder (vm-share) that contains the "Jenkins Config" and "Inventory.txt" files.

Establish two AWS instances, one for the JenkinsHost and another for the agent, both running and working as seen in the recording below.

Access the Vagrant machine using SSH command and moved the shared folder to the Agent using rsync.

Once in the agent vm i looked for the "vm-shared" folder which contained my playbooks.

When inside the correct folder i ran the command "ansible-playbook -v jenkins-config.yml -i inventory.txt" to run the playbooks.

Once it was completed, i used the public ip From the JenkinsHost machine from AWS with the port of "8080" in my browser to check if the Jenkins application was fully working


![demo](./Recording%202023-01-31%20at%2016.52.27.gif)