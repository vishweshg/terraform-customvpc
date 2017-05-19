## Terraform-Custom VPC
Here we will be creating a basic AWS VPC resources including the following:


* VPC
* Subnets (one private and two private)
* Routes
* Route Tables
* Elastic (EIP)
* Nat Gateway
* Route Association Table

Before we dive in, let’s explain the two concepts, what is Terraform and what is a VPC in AWS

#### Terraform

Terraform is a tool for building, changing, and versioning infrastructure safely and efficiently. Terraform can manage existing and popular service providers as well as custom in-house solutions.

Configuration files describe to Terraform the components needed to run a single application or your entire datacenter. Terraform generates an execution plan describing what it will do to reach the desired state, and then executes it to build the described infrastructure. As the configuration changes, Terraform is able to determine what changed and create incremental execution plans which can be applied.

The infrastructure Terraform can manage includes low-level components such as compute instances, storage, and networking, as well as high-level components such as DNS entries, SaaS features, etc.

#### VPC

VPC stands for Virtual Private Cloud. With a AWS VPC you decide on how your network will look like and then you get to build it in the way that suits you well, for example, you get to choose the IP addresses you want, you can also decide on how to break down your VPC into subnets by having for instance non internet-facing subnets (Private subnets) and internet-facing subnets (Public subnets). 

#### Requirements

--> Let’s now install Terraform

Go to the following URL https://www.terraform.io/downloads.html to download Terraform according to your OS, in this tutorial I am using Linux.

#### Setup

--> Let’s get-started

- Clone the repository
 
- Customize the IP to ur needs vpc.tf file
 
 -->Give the command

       $terraform apply
 
 Thats it!Once you give this command it will ask for access key and secret keys.After giving the credentials it will setup the custom vpc.
