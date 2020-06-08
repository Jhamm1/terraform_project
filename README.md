# terraform_project
Learning terraform 


Defines infrastructure as code

Spin up cloud resources

Sorts out resource ordering

blueprint for spinning up and managing your cloud resources

Step-by-step script to make changes in a certain order

Terraform uses a graph data structure (specifically, it uses Directed Acyclic Graph)

- Graph is made of of connected nodes
- Each node is a resource e.g. AWS s3, DNS and EC2
- The graph is direct as it is done in order
- This data structure is used to manage complexity under the hood

States

terraform plan -destroy -out=example.pln

terraform show example.pln

`vim terraform.tfstate` -  details about the infrastructure

`terraform state show aws_s3_bucket.tf_course` - state of cloud resources

`terraform show -json`

__Terraform graph__

`terraform graph` -  Graphic representation of infra

Take the ouput and enter it into http://www.webgraphviz.com/

`terraform plan -destroy -out=example.pln`

`terraform apply example.pln`

`terraform apply -auto-approve`

## Infrastructure as Code

### Resources

- Building blocks of Terraform code
- Define the "what" of your infrastructure and Terraform figures out the "how"
- Different settings for every provider
- Providers gives you access to resources



