# Hyperledger Fabric
2021-05-30 14:01:57 Sunday
## Install cURL
Command Line tool for transferring data using various network protocols. The name cURL stands for "Client URL".

`$ sudo apt update && sudo apt upgrade`

`$ sudo apt install curl`

Once the command line tool is installed, run the following command:
`$ curl --version`

## Install Docker
Docker is a set of platform as a service products that use OS-level virtualization to deliver software in packages called containers.

Use apt package manager to install Docker package.

`$ sudo apt update `

`$ sudo apt install docker.io`

Start and enable Docker service

`$ sudo systemctl start docker`

`$ sudo systemctl enable docker`

Check the status of Docker service and ensure that it is running. 
`$ sudo systemctl status docker`

### Configure user to work with Docker CLI

We need to add the user to docker group, so that the user can execute the docker commands.

`$ sudo usermod -aG docker prabusivakumar`

> **Note**: The changes will take effect in the new session. It is recommended that you logout and login to check if the user group 'docker' is added to user 'prabusivakumar'.

Let us verify the version of Docker installed.

`$ docker --version`

## Install Docker Compose

Docker Compose is a tool for running multi-container Docker applications.

`$ sudo apt update`

`$ sudo apt install docker-compose`

## Install Go
Go is a statically typed, compiled programming language. Use apt package manager to install Go Language Package.

`$ sudo apt update`

`$ sudo apt install golang`

Let us verify the version of Go installed.

`$ go version`

## Install NodeJS
Node.js is an open-source, cross-platform, back-end JavaScript runtime environment. Install Node Package Manager (npm) 

`$ sudo apt update`

`$ sudo apt install nodejs`

`$ sudo apt install npm`

Let us verify the version of Node.js and npm installed.

`$ node --version`

`$ npm --version`

Let us verify the version of Node Package Manager installed.

`$ node --version`

## Install Python
Python is an interpreted, high-level, general-purpose programming language.

`$ sudo apt update`

`$ sudo apt install python`

Let us verify the version of Python installed.

`$ python --version`

## Deploying Hyperledger Container

Download the latest version of the Hyperledger bootstrap.sh using the following command:

`$ curl -ssL https://raw.githubusercontent.com/hyperledger/fabric/master/scripts/bootstrap.sh > bootstrap.sh`

`$ ./bootstrap.sh`

The **fabric-samples** are downloaded to the current directory. 

Add the fabric-samples/bin folder to the **PATH** environment variable.

`$ export PATH=$PATH:$HOME/Hyperledger/fabric-samples/bin`

`$ cd ~/Hyperledger/fabric-samples/fabcar/javascript`

`$ npm update`

## Launch Hyperledger Fabric

Execute `$ ./startFabric.sh` to launch the Fabric.

`$ cd ~/Hyperledger/fabric-samples/fabcar`

`$ ./startFabric.sh`

`$ cd ~/Hyperledger/fabric-samples/fabcar/javascript`

`$ node enrollAdmin.js`

> Wallet path: /home/prabusivakumar/Hyperledger/fabric-samples/fabcar/javascript/wallet
Successfully enrolled admin user "admin" and imported it into the wallet

`$ node registerUser.js`

> Wallet path: /home/prabusivakumar/Hyperledger/fabric-samples/fabcar/javascript/wallet
Successfully registered and enrolled admin user "appUser" and imported it into the wallet



