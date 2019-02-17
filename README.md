# COnfiguring Jenkins to use .Net #

## Add a Windows node to Jenkins ##

1. Spin up a  Windows VM and Install Java
2. Jenkins -> Manage Jenkins -> Manage Nodes
3. Name the node and make it permanenant
4. Specify No. of executers Remot root directory
5. Specify Launch method as Launch agent via Java Web Start

** Step 5 not visible **
Jenkins -> Manage Jenkins -> Configure global Security -> Enable TCP port for JNLP agents fixed and port 3000

6. Go to the agent just configured and download the .jar file and move it to the remote directory on the agent
7. Run the commandd provided with the master ip and port giving the download .jar file as parameter
