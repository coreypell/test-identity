# Welcome to my Keycloak stack for local development and testing!

Please Read the instructions below to deploy the stack with docker-compose!

***NOTE: You will need docker/docker-desktop installed on your system before you attempt this***
_________________________________________________________________________________________________

**Create working directory, clone the repo, and build your images**

- ***Windows(PowerShell)***
  -  mkdir test-identity; cd test-identity
  -  git clone https://github.com/coreypell/test-identity.git .

- ***Linux/Mac***
  -  mkdir test-identity && cd test-identity
  -  git clone https://github.com/coreypell/test-identity.git .

__________________________________________________________________________________________________

**Deploy your stack!**

While you are still in the "test-identity" directory run:

  -  docker-compose up -d

The Docker Compose will build the images for you if this is your first time.
This will take some time, so please allow the process to complete!

From here you can navigate to https://localhost/auth to get to Keycloak.

_________________________________________________________________________________________________

Clean up!
  -  docker-compose down -v

The "-v" option deletes named volumes for a full cleanup!
If you wish to retain the named volumes, simply remove the "-v" option.

**Enjoy!**
