### Documentation Referred:

https://registry.terraform.io/

https://registry.terraform.io/providers/hashicorp/aws/latest/docs

### first_ec2.tf

```sh
provider "aws" {
  region     = "us-east-1"
  access_key = "ACCESS-KEY-HERE"
  secret_key = "SECRET-KEY-HERE"
}

resource "aws_instance" "jjtechec2" {
    ami = "ami-00c39f71452c08778"
    instance_type = "t2.micro"
}
```

### Commands:

```sh
terraform init
terraform plan
terraform apply
```
