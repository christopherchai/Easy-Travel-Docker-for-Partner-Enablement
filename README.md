# EasyTravel Docker for Partner Enablement
In this tutorial you will get a demo app (EasyTravel Docker) where you can deploy OneAgent from your Dynatrace SaaS tenant and get started on learning use cases on how to monitor applications and services with Dynatrace SaaS. The same will also work if you have Dynatrace Managed installed On-Premise. Also remember: Dynatrace can not only monitor your on premise apps but also your AWS Environments, Azure, OpenStack, OpenShift, VMWare or anywhere else!

## Target Audience
This tutorial is for you if:
1. You've just seen Dynatrace in action and would like to build up some hands-on experience with Dynatrace.
2. Nothing too deep, you just want to see what is Dynatrace.

## Pre-requisites
1. You need an AWS account. If you don't have one [get one here.](https://aws.amazon.com/)
2. You need a Dynatrace Account. Get your [Free SaaS Trial here!](http://bit.ly/dtsaastrial) If you already have one, then please proceed to use that instead of signing up a new tenant.

## Launch an EC2 Instance with EasyTravel Docker
In this lab we will launch an EC2 instance with built-in Docker application.

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

**Frequently Asked Questions**
1. *I can't access my website even though I have started up the EasyTravel application.*
   - Make sure you have the right security group assigned to your EasyTravel EC2 instance that allows inbound TCP HTTP 80 connection. For more information, please refer to https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-network-security.html.
2. *After starting up EasyTravel, I can see some WARNING messages appearing on my screen, should I be concern about it?*
   - Yes, it's perfectly normal to see these messages, it's part of the problem pattern of the application to be shown after you deployed Dynatrace OneAgent.
3. *Can I exit the SSH session and keep EasyTravel running?*
   - Yes, you can exit the SSH session and EasyTravel will keep running; it would only stop if you explicitly input Ctrl+C.

## Getting started with Dynatrace
In this lab you will get hands-on with basic navigation of Dynatrace. Download the **Getting Started with Dynatrace.pdf** attached in this repository and follow the instructions.

Happy Dynatracing!

Chris Chai (christopher.chai@dynatrace.com)
