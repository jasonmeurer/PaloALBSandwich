# Using VM-Series Firewalls and an LB Sandwich in AWS

LB Sandwich with 2 Firewalls and 2 Web Servers.

2 Options each with an ALB External. 

The alb internal requires PANOS 8.1 due to the use of the FQDN NAT Translated Destination.

**Documentation**

* [Deployment Guide](https://github.com/jasonmeurer/PaloALBSandwich/blob/master/ALB%20Sandwich%20Deployment%20Guide.pdf)

Refer to the API-Commands.txt file for a set of commands to update the address objects directly.

* About the [VM-Series Firewall for AWS](https://aws.paloaltonetworks.com)
