# README

Provide a basic configuration to describe an OpenStack Security Group with Terraform.

## Usage

```HCL
module "openstack_secgroup_ssh" {
  source = "julienlevasseur/security-group/openstack"
  name        = "std_ssh_rhel_base"
  description = "Wide SSH access"
  from_port   = 22
  to_port     = 22
  ip_protocol = "tcp"
  cidr        = "0.0.0.0/0"
}
```

## Authors

Julien Levasseur (https://github.com/julienlevasseur)