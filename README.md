# Install terraform
Please follow the instruction on the official website
https://www.terraform.io/downloads.html

# Config and start an example using nginx on docker
- Prerequisite : an installed docker (https://docs.docker.com/install/)
- Checkout the config.tf file
- use shell and place it on the config path
```shell
cd [config.tf path]
```
- 
```shell
$ terraform plan -out config.tfplan
```
- 
```shell
$ terraform apply
```
- 
```shell
$ terraform show
``` 

we can check the existing container using 
```shell
$ docker container ls
```
