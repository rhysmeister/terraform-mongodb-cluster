# terraform-mongodb-cluster

This Terraform module creates infrastructure for a MongoDB single-replicaset cluster along with a Bastion Host. After deployment of the infrastructure the Bastion Host should be used to install MongoDB and setup the replicaset.

# module structure

* ansible/ - Contains Ansible resources for deployment of MongoDB on the infrastructure.
* examples/ - Contains examples for using the module.
* modules/ - Contains nested modules
  * terraform-mongodb-cloudwatch - Cloudwatch Alarms for the MongoDB Instances.
  * terraform-dba-bastion - Bastion host for the MongoDB Cluster.
  * TODO
* main.tf
* outputs.tf
* variables.tf
