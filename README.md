# Easy Travel Docker for Partner Enablement
In this tutorial you will get a demo app (EasyTravel Docker) where you can deploy OneAgent from your Dynatrace SaaS tenant and get started on learning use cases on how to monitor applications and services with Dynatrace SaaS. The same will also work if you have Dynatrace Managed installed On-Premise. Also remember: Dynatrace can not only monitor your on premise apps but also your AWS Environments, Azure, OpenStack, OpenShift, VMWare or anywhere else!

## Pre-requisites
1. You need an AWS account. If you don't have one [get one here](https://aws.amazon.com/)
2. You need a Dynatrace Account. Get your [Free SaaS Trial here!](http://bit.ly/dtsaastrial)

## Launch an EC2 Instance with EasyTravel Docker
In this lab we will launch an EC2 instance with built-in Docker application 

**Step by Step Guide**
1. Log into to AWS console.
2. Select EC2 and Click on Launch an Instance. Make sure you are launching the EC2 instance in Asia Pacific (Singapore) region.
3. Click on Community AMI's. In the Search box type **EasyTravel Docker for Partner Enablement**. There should be only one image with the following description: "EasyTravel Docker installed and pulled, can be run immediately".
4. Select **t2.medium** instance type, explore the options and launch the EC2 instance.
5. SSH into the EC2 instance, login with username: perform, password: perform
6. Use the following commands to start EasyTravel Docker
   - cd easyTravel-Docker/
   - docker-compose up
7. Now you can access EasyTravel Web UI via http://<EC2_instance_public_IP>.
8. To stop EasyTravel Docker, simply input Ctrl+C.

## Getting started with Dynatrace
In this lab you will get hands-on with basic navigation of Dynatrace. Download the Getting Started with Dynatrace.pdf attached in this repository and follow the instructions.

Happy Dynatracing!

Chris Chai (christopher.chai@dynatrace.com)
