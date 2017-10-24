# Uqi's Technology Choices

This is a collection of technology pieces that have been performed excellently during my career, or I am excited about.
This is inspired by [Thoughtworks Technology Radar](https://www.thoughtworks.com/radar), and I am trying to add local touches
to it.

_Disclaimer_ : This is my personal opinion and does not reflect any of the company i am working on.

## Data Center and Infrastructure

### 1. Data Center: No one

So far I have NOT found working on a data center in Indonesia that is satisfying. 
I only worked on 2 data centers in Indonesia, which are Biznet Midplaza and Biznet Technovillage.
Biznet Midplaza has great connectivity from ISP, but the power source only comes from one grid.
Biznet Technovillage have great location and expansion, as well as belong to Tier 3. But the ISP choice is limited.

### 2. ISP: Biznet

I can however, vouch on Biznet as an ISP. They have great support and team, and provides many connectivity.
They are excellent both as Internet and WAN connectivity provider.

### 3. Rack: APC

APC Netshelter SX is my choice for rack. It comes with variety of sizes and accessories, such as
cable managers, power strips, etc. I will always use this instead of any racks comes as a standard from the data center.

### 4. Server: Dell Poweredge

Dell servers have great management called iDRAC which I like.

### 5. Server: Supermicro

Supermicro server design really stands out among its competitors, particularly their Ultra, BigTwin, and Simply Double line.
They are also a great value compared to big brands, although their exotic line has comparable price.

### 6. UTP Cables: Eco Patch

[EcoPatch](https://www.ncj.co.jp/product/product-ecopatch.php) is a great cable which is unbeliveably thin.
Unfortunately they are only available in Japan, and importing here costs a fortune.

### 7. Firewall: No one

Firewalls like Cisco are great, but sometimes they comes with nasty bug like losing your ARP table after 213 days.
Not Fortinet as well, because the VPN needs propetiary protocol and client, and it disconnect with OS X quickly.

### 8. Routers: No idea

I hope i can touch this some time.

### 9. Switches: No idea

Same as routers.

### 10. IT Distributor: Berca

Berca has responsive, great sales and great price.

### 11: Storage: No idea

Unfortunately, I have not worked with storage solutions yet.

## Platform and Devops

### 1. IaaS: AWS

AWS is still the benchmark for the infrastructure provider, although it gets more complex and expensive each day.
It has many features and SaaS add-ons. It is also very easy to find engineers who are familiar with AWS.

If you want to deploy in AWS, I would recommend Tokyo (ap-northeast) Region since it has 3 availability zones. This is critical
when you are deploying services that requires quorum.

I also had experience with local IaaS, most of them are lacking in features such as providing high IOPS or lacking in usability.
Hopefully this will change in the future.

### 2. Monitoring: Datadog

I really like Datadog because it has great choice of third party profiling. They are also quite a bit cheaper than NewRelic.
When you want to use its custom metrics, make sure to architect it to be pulled instead of push to ease transition to open source 
alternatives.

### 3. Monitoring: Prometheus

Prometheus is great once your services / server count reached > 150 and your Datadog bill is killing your budget.
Setting it up is a little bit complex though, and the alerting is not as easy as Datadog.

### 4. Container Orchestration: Kubernetes

Kubernetes has great features for container-based infrastructure. It is very active. I only compared with Rancher for 1 year, 
but at the end I put my choice on Kubernetes.

### 5. Service Discovery: Consul

Consul has innovative protocol for service discovery, and setting it up also really easy.

### 6. Logging: Graylog

Graylog is awesome for logging. Setting it up is really complex, but once it is running, it is cheaper than Splunk and has great features
and plugins.

### 7. Full Text Search: Elastic Search

Having Elastic Search experience is essential for your team to handle searching problem.

### 8. Infrastructure Automation: Ansible

Ansible is very simple for automating infrastructure. 

### 9. Application Packaging: Docker

Docker provides excellent packaging and isolation for your container.

### 10. Repository: Gitlab

Having Gitlab can reduce your Github company bill.

### 11. CI: Gitlab CI

Gitlab CI is amazing because you can put workers that can pull from Gitlab server itself.

### 12. Server OS: Ubuntu

I guess if I have to choose only one base operating system for all of my servers, it would be Ubuntu. But of course,
you mix and match your OS based on your needs.

### 13: HTTP Manipulator: Kong

Kong is excellent to manipulate your HTTP requests.

### 14: Hypervisor: KVM

Although there are many excellent supervisors out there, I really like KVM. It is free and easy to setup. It is also the base
for more complicated setup such as Proxmox or Openstack.

### 15: Relational Databases: MySQL

I actually don't like MySQL very much, it is that I have most exposure compared to other relational DBs like Postgre and Oracle.
It comes with various flavors, the one I like most is Percona ones because there are a lot of other toolings around it.

### 16: Messaging: Kafka

Kafka is a very fast messaging system and very easy to configure. It is very complex to set up the operational tools around it,
however it is pretty maintenance-free once it is going.

### 17: Platform Architecture: One subnet for one module

If we really need subnetting, better add one subnet for each module, and apply ACLs based on that.

## Programming and Architecture

### 1. Programming Language: Java

Java is still de-facto language in enterprise that needs speed. Nuff said.

### 2. Architecture: Monolithic to Microservices

Start from monolithic, then break up to microservices. Microservices need a lot of tooling to be resilient, 
such as Kubernetes, Kafka, Kong, Consul.

### 3. In-memory Data Store: Redis Sentinel / Redis Cluster

Never go with only single redis, unless it is ok to have data loss / cache rebuild. For HA setup, use Sentinel
for low throughput and low volume, and Cluster for high throughput / fast growing storage.