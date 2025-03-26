# Project 2 – Hybrid Cloud Backend Architecture with Private RDS

## Overview
Simulates a backend cloud environment with a public EC2 server securely connecting to a private PostgreSQL RDS instance. All traffic routed via AWS VPC networking components.

## Key Features
- VPC with public and private subnets
- DB Subnet Group for RDS
- EC2 (Amazon Linux 2) in public subnet
- PostgreSQL RDS (v17) in private subnet
- NAT Gateway + Internet Gateway
- Security Groups for strict inbound/outbound control

## Troubleshooting Wins
- CIDR overlap fix
- RDS access via SSL using `sslmode=require`
- Password auth and user conflicts resolved
- EC2 Security Group recreated after deletion

## Outcome
Connected EC2 to private RDS securely and confirmed psql shell access. Architecture is scalable, secure, and production-similar.

## Example Command
```bash
PGPASSWORD='yourpassword' psql "host=<rds-endpoint> user=<username> dbname=postgres sslmode=require"
```
