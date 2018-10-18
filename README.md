## Jenkins
This project is based on the official [Jenkins Docker Store](https://hub.docker.com/r/jenkins/jenkins/) image.

### Server

After cloning this repo, start by executing

	docker-compose up
		
To shut down the server, execute

	docker-compose down
		
**Note:** the previous command will leave the `jenkins_home` volume as is. Currently all the server configuration data is kept in this location.

To shut down the server and simultaneously remove the volume, execute

	docker-compose down -v

**TO DO:**

1. Test the initial image and add Sizmek-specific configuration to it.
2. Create the executor image creation code and add it here.
3. Add BATS tests for both server and executor.
4. Documentation for the Jenkins infrastructure will be maintained in this README.

