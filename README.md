# Project 1 – Public Web Architecture on AWS (EC2 + Apache)

## Overview
Deployed a public-facing Apache web server using Amazon EC2 within a custom VPC and public subnet. Designed for quick access and real-world exposure to AWS fundamentals.

## Key Features
- Amazon EC2 (Amazon Linux 2)
- Apache HTTP server setup via terminal
- Public subnet with Internet Gateway
- Port 22 and 80 open via Security Groups

## Outcome
Successfully hosted and accessed Apache welcome page from the internet. Built VPC manually and deployed EC2 into a secure, internet-accessible environment.

## Commands Used
```bash
sudo yum install -y httpd
sudo systemctl start httpd
sudo systemctl enable httpd
```
