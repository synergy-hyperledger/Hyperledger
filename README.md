# Hyperledger Fabric (Prerequisite)
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
Node.js is an open-source, cross-platform, back-end JavaScript runtime environment. 

`$ sudo apt update`
`$ sudo apt install nodejs`

Let us verify the version of NodeJS installed.

`$ node --version`

## Install Python
Python is an interpreted, high-level, general-purpose programming language.

`$ sudo apt update`
`$ sudo apt install python`

Let us verify the version of Python installed.

`$ python --version`
