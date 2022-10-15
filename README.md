# Deploying software to a VPC 

## Overview

The goal of this project is to utilize Jenkins' ability to have hosts in order to deploy to another VPC. The build of this pipeline is not optimal at all, in an ideal situation instead of deploying to another VPC entirely you would transfer within subnets of the same VPC. The reason for the approach taken in this repository is to test the concept of transferring data across different VPCs.

## Step by Step guide

1. Install Jenkins and required packages to an EC2.
2. Install Nginx, JRE, Python3-venv and python3-pip to another ec2.
3. Set up the second ec2 as an agent
4. Configure the Nginx sites-enabled/default file
5. Configure the email notification plugin for Jenkins.
6. Install Jenkins' Keep Running plugin.
7. Deploy this application - the expected result will be a url shortener. 
