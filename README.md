# Dosa and Drinks

## The Problem

A restaurant website needs to load fast, be secure, and stay up even when something goes wrong. If the site goes down, customers can't see the menu or find the place. The goal was to design the site and build AWS infrastructure that keeps it running no matter what.

## What I Did

- Designed the Dosa and Drinks website
- Hosted it on Amazon S3 and sped up loading with CloudFront
- Set up the domain with Route 53 and HTTPS with an SSL certificate from ACM
- Controlled access with IAM
- Ran the site on two EC2 servers behind an Application Load Balancer
- Managed the servers and pushed content updates with EC2 Instance Connect and the AWS CLI

## Result

I tested failover by shutting down one server on purpose. The load balancer automatically sent all traffic to the healthy server and the site stayed up with no downtime.

## Tools

AWS S3, CloudFront, Route 53, ACM, IAM, EC2, Application Load Balancer, AWS CLI

Watch the demo: https://youtu.be/9lcx_JJ3BvY
