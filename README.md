Terraform Module to provision an AWS EC2 instance with the latest amazon linux 2 ami and installed docker in it.

Not intended for production use. It is an example module.

For instance aws

It is just for showing how to create a publish module in Terraform Registry.

Usage:

```hcl

provider "aws" {
  region = "us-east-1"
}

module "docker_instance" {
    source = "bekirbilgec/docker-instance/aws"
    key_name = "yunusemre"
}
```