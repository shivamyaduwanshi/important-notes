# Installing Node.js on an AWS EC2 Ubuntu Instance

This guide will show you how to install Node.js on an AWS EC2 Ubuntu instance.

## Connect to your instance

1. Connect to your AWS EC2 Ubuntu instance via SSH.

## Update the package lists

2. Run the following command to update the package lists:
sudo apt-get update

## Install Node.js and npm

3. Run the following command to install the latest version of Node.js and npm:
sudo apt-get install -y nodejs npm

## Verify the installation

4. Verify that Node.js and npm are installed by checking the version:
node -v
npm -v

5. You can also check if Node.js is running by creating a simple test file, for example `test.js` and type in 
console.log("Node.js is running!");

6. To run this file type 
node test.js

7. You should see "Node.js is running!" in the terminal

You can also use Node Version Manager(nvm) to manage multiple versions of Node.js on your system.

This will install Node.js and npm on your AWS EC2 Ubuntu instance. You can now use npm to install packages and run your Node.js applications.

Please note that, you should also keep your Node.js version up-to-date to receive security updates.
