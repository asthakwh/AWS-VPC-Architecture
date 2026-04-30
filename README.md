AWS-VPC-Architecture

step1: create Vpc with choosen ip address range
Example= 172.31.0.0/16

it also defined by CIDR value includes 65531


step2: create subnet

Public Subnet: 172.31.1.0/24 (web server EC2 activity)
Private Subnet: 172.31.2.0/24 (Database server Connectivity)

step3: create Internet Gateway 
IGW-Attach to VPC

step4: create Route Tables (also aws create default route table)

Public subnet route: add = 0.0.0.0/0 (Internet Access)
Private subnet: No direct internet access
