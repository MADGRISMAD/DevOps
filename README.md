# DevOps

This repository is used for iTjuana DevOps Bootcamp

## To build the docker file in "capstone_project/hello-world"
### cd capstone_project/hello-world
### docker build -t my-react-app .

## To run the docker file in "capstone_project/hello-world"
### cd capstone_project/hello-world
### docker run -p 3000:3000 my-react-app

## To update the node js application to display "Hello DevOps!" instead of "Hello World!" using ansible.
### cd ansible-challenge/
### docker-compose up

## Open a new terminal and get into the controller machine
### sudo docker exec -w /home/ansible_controller/capstone_project/hello-world/ -ti ansible_controller bash
### ansible-playbook -i inventory.ini update-nodejs-app.yml
