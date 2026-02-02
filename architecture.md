# AWS VPC Architecture

## VPC CIDR
- 10.0.0.0/16

## Subnets
| Name | CIDR | Type |
|----|----|----|
| Public Subnet | 10.0.1.0/24 | Public |
| Private Subnet | 10.0.2.0/24 | Private |

## Gateways
- Internet Gateway → Public Subnet
- NAT Gateway → Private Subnet

## Security
- Public EC2 accessible via SSH
- Private EC2 accessible only via Public EC2
- No public IP on private instance
