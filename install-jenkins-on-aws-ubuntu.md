# Install Jenkins on AWS EC2 Ubuntu
1. Connect to your AWS EC2 Ubuntu instance via SSH.
2. Add the Jenkins repository to the sources list by running the following command: `wget -q -O - https://pkg.jenkins.io/debian/jenkins.io.key | sudo apt-key add - && sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'`
3. Update the package lists by running the following command: `sudo apt-get update`
4. Install Jenkins by running the following command: `sudo apt-get install jenkins`
5. Start the Jenkins service by running the following command: `sudo systemctl start jenkins`
6. Verify that Jenkins is running by typing the following command: `sudo systemctl status jenkins`
7. You can also check if Jenkins is running by visiting the server's public IP on port 8080 in your web browser. You should see the Jenkins login page.
8. To setup the initial password for Jenkins, you can use the following command: `sudo cat /var/lib/jenkins/secrets/initialAdminPassword`
9. Now, you can unlock Jenkins.
