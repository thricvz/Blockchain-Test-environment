### TEST ENVIRONMENT FOR BLOCKCHAIN PROJECT

The following repository is auxiliary to my blockchain implementation project as it contains a simple test network implemented with the help of docker containers.
The user is free to add new machines to this virtualized network by editing the ``docker-compose.yaml`` file.
**Please note that for the new node to be taken in account it must have either of these two custom docker images:**
- reliable-node (meant only for nodes that are always active on the network)
- simple-node 

## Pre-requisites
- Docker & Docker-compose

## Launching the Test Environment

First, modify the permissions of the ``prepare-env.sh`` with the ``chmod +x prepare-env.sh`` command.
Second, execute the script with privileged rights: ``sudo prepare-env.sh``

These steps allow us to successfully build our custom docker images,that are required in our docker-compose config file

Finally,execute ``docker-compose up`` to start our test environnment! 
