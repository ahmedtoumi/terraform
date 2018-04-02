## Intro
In this Example we will create an internate gateway on aws, a web VPC attached to this gateway and an other VPC for databse that could not be acceded from internet (only from web VPC).


## Prerequisites
- Install terraform
- already have an admin AWS account (access key and secret)
- execute that using your own tokens :
```shell
> export AWS_ACCESS_KEY_ID="your AWS key id"
> export AWS_SECRET_ACCESS_KEY="your AWS secret key"
```

## Test And Execute
- check if terraform provider is already installed and if configuration is good
```shell
> cd [this project folder]
> terraform plan
```

- create AWS plateforms (executing the terraform plan)
```shell
> terraform apply
```

I have added an output to see the pûblic IP affected to have access to web VPC through the gateway, you can use it to test if the pache server respond
or you can use it to your ansible host configuration to prepare some playbooks.

Finally don't forget to destroy all AWS VPCs ... because it's money spent ...
```shell
> terraform destroy
```
