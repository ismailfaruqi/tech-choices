# Uqi's Technology Choices

This is a collection of technology pieces that have been performed excellently during my career, or I am excited about.

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
cable managers, power strips, etc. I would not use any standard racks that is coming from the data center,
instead I will use this.

### 4. Server: Dell Poweredge

Dell servers have great management called iDRAC which I like.

### 5. Server: Supermicro

Supermicro servers, particularly the BigTwin line, give the highest computing power density without blade complexity.
They are also a great value compared to big brands, although their exotic line has comparable price.

### 6. UTP Cables: Eco Patch

[EcoPatch](https://www.ncj.co.jp/product/product-ecopatch.php) is a great cable which is unbeliveably thin.
Unfortunately they are only available in Japan, and importing here costs a fortune.

### 7. Firewall: No one

Firewalls like Cisco are great, but sometimes they comes with nasty bug like losing your ARP table after 213 days.

### 8. Routers: No idea

I hope i can touch this some time.

### 9. Switches: No idea

Same as routers.

### 10. IT Distributor: Berca

Berca has responsive, great sales and great price.

## Platform and Devops

### 1. IaaS: AWS

AWS is still the benchmark for the infrastructure provider, although it gets a little complex and expensive.
It is also very easy to find engineers who are familiar with AWS.

### 2. Monitoring: Datadog

I really like Datadog because it has great choice of third party profiling. They are also quite a bit cheaper than NewRelic.
When you want to use its custom metrics, make sure to architect it to be pulled instead of push to ease transition to open source 
alternatives.

### 3. Monitoring: Prometheus

Prometheus is great once your services / server count reached > 150 and your Datadog bill is killing your budget.
Setting it up is a little bit complex though.

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

I guess if I have to choose only one operating system for all of my servers, it would be Ubuntu.

### 13: HTTP Manipulator: Kong

Kong is excellent to manipulate your HTTP requests.

## Programming and Architecture

### 1. Programming Language: Java

Java is still de-facto language in enterprise that needs speed. Nuff said.