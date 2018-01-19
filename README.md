# selenium-grid-docker
# Deploying a slenenium grid with docker

Installing Ubuntu basics

The Dockerfile


### Start the grid with the default. View docker-compose.yml and edit to change.
        docker-compose up -d

### Scale up by adding more nodes. this example adds 3 more chrome and 4 firefox nodes
        docker-compose scale chrome=3
        docker-compose scale firefox=4
        
### Destroy! Take the grid down.
        docker-compose down
        
### Combine up and scale to start with more than the default
        docker-compose up -d --scale firefox=4 --scale chrome=3
        
###  View the docker images running
        docker-compose ps
        
### Load the grid console in browser to see the nodes you have registered.
  Examples:
  http://localhost:4444/grid/console
  http://seleniumgrid.westus.cloudapp.azure.com:4444/grid/console
