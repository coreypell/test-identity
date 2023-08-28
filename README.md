Welcome to my Keycloak stack for local development and testing!

Please Read the instructions below to deploy the stack with docker-compose!

**NOTE: You will need docker/docker-desktop installed on your system before you attempt this**

Create working directory, clone the repo, and build your images

  -  mkdir test-identity && cd test-identity
  -  git clone https://github.com/coreypell/test-identity.git .
  -  docker build -t test-apache:latest ./test-apache
  -  docker build -t test-keycloak:latest ./test-keycloak
  -  docker build -t test-postgres:latest ./test-postgres


Deploy your stack!
While you are still in the "test-identity" directory run:

  -  docker-compose up -d

From here you can navigate to https://localhost/auth to get to Keycloak.

Clean up!
  -  docker-compose down

**Enjoy!**
