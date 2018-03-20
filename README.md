# Using VM-Series Firewalls and an ALB Sandwich in AWS
ALB Sandwich with 2 Firewalls and 2 Web Servers


Requires PANOS 8.1 due to the use of the FQDN NAT Translated Destination

Instructions

0. Create the Bootstrap bucket place the Bootstrap.xml and init-cfg.txt files into the Config folder.
	* [Creating the Bootstrap Bucket](https://www.paloaltonetworks.com/documentation/71/virtualization/virtualization/bootstrap-the-vm-series-firewall/bootstrap-package)
1. Deploy the CFT
2. Launch a Jumpbox into either NATGateway Subnet.
3. Access the Jumpbox to gain access to the Firewall GUIs.
	* Username/Password - pandemo/demopassword
	* The CFT creates a sgJumpbox Security Group for use allowing ports 22 and 3389.
4. Update the "alb-internal" object with the FQDN of the Internal ALB available on the Outputs of the CFT.
5. Update the "AWS-NAT-UNTRUST" object with the Firewall's Untrust IP address available on the Outputs of the CFT.
6. Test access do the External ALB FQDN.


**Documentation**
* Release Notes: Included in this repository.
* About the [VM-Series Firewall for AWS](https://aws.paloaltonetworks.com)
