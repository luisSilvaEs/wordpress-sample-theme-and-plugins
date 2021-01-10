# ABOUT this repo

## This repo contains:

- A Docker image with a Wordpress environment ready to be deployed

## How to install docker initially
This step is not necessary when pull project from git

IMPORTANT, there are 2 ways to install Wordpress using docker:

- Execute the following command:
` docker pull wordpress `

or 

- Using a docker-compose file, which is the procedure we use for this repo. It consists in the following:

 * Create an empty docker-compose.yml file inside the folder, on it we will copy and paste the content from this repo [Sample docker file](https://github.com/docker/awesome-compose/blob/master/wordpress-mysql/docker-compose.yaml)
 IN case an error related to the 80 port indicating it is already in use, just change port number in the line 22 to 8086, 8088 or another available
 * Execute in terminal the following line: `docker-compose up -d`
 * After executing the previous command, you should see indicated in the terminal or in the Docker dashboard the 2 volumes as done (Terminal) or in green color (Dasdboard) ![Image](volumes-installed.png "icon")
 * Finally, open your browser and go to the following URL: localhost:80 to the Wordpress app running

##### Reference
[Docker image](https://hub.docker.com/_/wordpress)
