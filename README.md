# Deploy 

Deploy your Check Point (and some others) infrastructure in the cloud with simple scripts and templates. 

Commands must be run from the home directory /ctrl (cd ~)

Follows a simple pattern of action/target, used to test three states of infrastructure.


### 1. Configure your instance

cfg
|── mg => configure Check Point management station for autodeploy
|── openstack
|── secvpc => configure a vpc and gateway to secure it
|── ubuntu


### 2. Launch your instance

create
|── mg => launch SmartCenter instance
|── openstack
|── secvpc => configure new VPC and launch gateway
|── ubuntu


### 3. Delete your instance

destroy
|── gw
|── mg => delete your running instance
|── openstack
|── secvpc => delete gateway and remove VPC configuration
|── ubuntu

