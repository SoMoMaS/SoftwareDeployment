# SoftwareDeployment

## MySQL

- Added new working directory 
- added new Dockerfile 
- Created bash script for secure installiation of mySQL
- MySQl Init file added

## Wordpress 
- Dockerfile added
- Entry point script created

## Build
After I added the compose file on the root folder which combines the MySQL DB image and the Wordpress + apache + PHP image, 
I needed to run the following script to build both images 

```
docker-compose up -d
```

