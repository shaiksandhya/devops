In 3-tier application we have

web/frontend tier
app/api/backend tier
db tier

In AWS, we have Regions, AZ(Availability Zones)
AMI- Amazon Machine Image  (These are like our operating Systems)

In AWS mostly resources are regions based, only few services are global.

Global Services Example : S3, IAM
Regional Based services: Ec2

AZ is for High Availaility purpose, instead of creating the resources in one AZ we can place the infra in multiple AZ's. If something wrong with one AZ, we can access our infra from another AZ.

HA(High Availability) - we can create resources in atleast 2 AZ's
DR(Disaster Recovery) - we can move the resources to another region or another AZ.

Here in this application we frequently use nginx.

OS + Install package + configure service/package

We can create the instance and install the nginx , create the image out of it.

We can create the image when the server is stable or its running

stable vs running

when server is running, by the time you take photo of server, many things may happen. it leads to errors.

Windows OS + install MS office + Anti virus = Windows-10.iso

The below os has almost common features

centos8 = AWS Linux 2 = RHEL8 = Fedora

When we are implementing the Application frfom the scratch.

What programming languages and
What are the tools and versions of programming will be decided by the Developers and Architects.

DevOps tools will be decided by the DevOps Architects.

Developer write the code --> compile --> build/package
if it is java
java -> .jar
.net - dll
all languages --> .zip

RDBMS --> SQL --> Relation Database management system -->It has Rows and Columns
NoSQL --> No SQL -> no tables no rows and columns --> data is based on documents and collections --> js files

By default some servers mostly DB servers, you can't open them apart from local server. this is for security


system/service user
-------------------
user --> human
system(non-human) --> on behalf of users, applications have dedicated users for security

install dependencies/libraries --> 
maven --> pom.xml
nodejs/js --> package.json
requirements.txt --> python


Google the below Topics

What is FFirewall?
What is VPN?
RDBMS vs NoSQL
Forward vs Reverse proxy


