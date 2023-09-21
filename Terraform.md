
Infrastructure
---------------

Infrastructure as a code --> IaaC/IaC

Terraform is very popular IaaC Tool.

Terraform follows the below principle.

DRY --> Dont Repeat Yourself

common --> we can use it wheneever required, central 

advantages
--------------

1. version control

	since terraform is a code, it should be kept in version control, so that we can maintain the history and we can revert to previous version if something goes wrong.

2. consistent infra

	same terraform code you run against multiple env, so all env is exactly same.

3. CRUD --> create read update delete

4. inventory management

	by seeing terraform, you can say what are the services and resources you are using for a particular project.

5. cost optimisation...

	when you need you create infra, when not required you delete the infra

6. dependency management

	Ec2 --> Security group
	first create security group and then create Ec2
	Ec2, sg code

7. modules --> reuse the code..

imperative/declarative

terraform is popular declarative scripting for infrastrcuture automation. easy syntax, no need of sequence execution, we will get it whatever we write if we follow syntax
