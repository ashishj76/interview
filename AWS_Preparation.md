# What is AWS
Amazon Web Services is a cloud services platform and is a subsidiary of amazon
AWS allows individuals and business both large and content to scale through compute power, online storage and content delivery on a pay as you go basis
AWS provides services for online storage and delivers dynamic and static content globally.
With AWS you can create any online application you require. AWS is a leader amongst cloud providers allowing its users to become more agile

# Tell about yourself and why you want to work in AWS role
I have always been someone who is technically minded and over the years I have built up a wide array of skills, qualities and experience that will enable to  excel within AWS position.
Just some of the skills and qualitied I possess include an understanding of AWS, its uses, best practices and procedures, proficiency in cloud based applications using AWS, an understanding of s3, AMI, EC2, SQS, and also how all of these integrate with AWS.
I am able to work well both on my own and as part of team and I can be relied upon to work quickly, to a high standard and also within strict timelines.
If hired, I will always work hard to help achieve commercial objectives and follow Amazon leadership principles in everything I do. 

# Why you want to work for Amazon?
I would like work for amazon not only because it is only one of the greatest companies in the world, but also desire to continually innovate, create and design ground breaking products and services.
I am type of person who doesn’t want to sit still in my job and just do bare minimum. I want to constantly evolve, improve and learn the skills and experience I have gained.
Amazon will continue to thrive as it puts customers at front of everything it does. For those reasons I feel immensely proud to work for Amazon in this AWS position. 

# What are the core services/components on AWS?
There are many components or services that AWS offers. The core ones can be broken down into storage, management, security, databases, mobile services, application services, networks and analytical services.
Some of the standout components are EC2 - which provides scalable compute capacity in cloud. VPC allows users to create their own virtual private networks where they have complete control to launch any AWS services.
There are many services in storage that AWS offers such s3, EBS. Databases are also key component of AWS with services such as RDS which enables the quick setup and use of rational database via the cloud.
AWS also provides, SWS (Simple Workflow services) for task management, SQS for automation. AWS also provides array of management services such as CloudWatch and CloudTrail for debugging. 
Compute
	- Lambda
	- EC2
	- AutoScaling
	- Elastic BeanStalk
Storage
	- S3
	- Glacier
	- EBS
	- EFS
Networking
	- VPC
	- CloudFront
	- Route53

# What is Geo Targeting and how you setup in CloudFront
	- It is concept where you can show personalized content to the users based on the geographoc location without chnaging the Url
	- AWS allows to send the customized ontent thru cloudfront
	- CloudFront delivers the content to end user at high speed and with low latency
	- CloudFront detect the country and forward the country code as origin server in header CloudFront-Viewer-Country

# Steps involved in CloudFormation
	- Create template in JSON/YAML
	- Save code in S3
	- Use AWS Cloudformation to create the stack
	- It will create the stack in the order which is defined in the templates. It will create the dependent resources first. In case of failure it will rollback

# Upgrade/downgrade the system with near 0 downtime (vertical and horizontal scaling)
	- Start ec2 console with required configuration
	- Add new machine in autoscaling
	- Terminate the old one

# Tools to analyze cost in AWS
	- AWS Cost dashboard - Table shows the top free service by usage
	- AWS Cost Explorer - will allow to analyze the pattern and can forecast in coming months
	- AWS Budgets - plan your service usage, costs and will alert once budget is reached
	- Cost Allocation Tags - helps if finding the which team/resource is costing

# Services can be used to create centralized logging solution
	- CloudWatch
	- Kinesis
	- S3
	- Elastic Search
	- Cloud Trails - History of API calls for every account.

# How do you setup Monitoring
	- CloudWatch helps to monitor application status of various services  and events
	- It can monitor
		○ State changes in EC2
		○ AutoScaling lifecycle events
		○ Scheduled events
		○ API calls
		○ Console sign-in events
	
# Define regions and availability zones in Amazon EC2.
Amazon web service has a global infrastructure that is divided into availability zones and regions. Each region is divided into a geographic area and it has multiple isolated locations called availability zones.

# What are the layers available in cloud computing?
Ans:  Below listed are the various layers of cloud computing
SaaS: Software as a Service 
PaaS: Platform as a Service
IaaS: Infrastructure as a Service
DaaS: Data as Service

# Explain the various storage classes available in S3? 
	- Standard frequency accessed 
	- One-zone infrequency accessed 
	- RRS - reduced redundancy storage
	- Standard infrequency accessed 
	- Glacier

#  What are the methods to encrypt the data in S3? 
	- Server-Side Encryption - C 
	- Server-Side Encryption - S3 
	- Server-Side Encryption - KMS     

#  What is the difference between EBS and S3?
EBS         	                    S3
Highly scalable	                    Less scalable
It is a block storage	            It is an object storage
EBS is faster than S3	            S3 is slower than EBS
User can access EBS only via 
the given EC2 instance	
Anyone can access S3;               it is a public instance.
It supports File system interface	It supports Web interface

# What is RTO and RPO
	- RTO - Recovery Time Objection. It is the maximum time your company is willing to wait for the recovery to finish in case of an outage.
	- RPO - Recovery Point Objective. .It is the maximum data loss company is willing to accept as measured in time. 

# What is the difference between CloudFormation and Elastic Beanstalk
CloudFormation	Elastic Beanstalk
Helps you describe and provision all the infrastructure	It provides and environment where you can easily deploy  and run application in 
 resources in the Cloud environment. 	Cloud.
It supports the infrastructure needs of many different types  of application	It Is combined with developer tools and helps you manage the lifecycle of the application.
Such as enterprise, legacy  etc.

# How to use AWS WAF in monitoring AWS application?
	- AWS Web Application Firewall protects your web applications from common web exploits.
	- Helps control which traffic source to application should be allowed or blocked. 
	- We can use WAF to create custom rules that block the common patterns.
	- WAF can be used for 3 cases - allow aall requests, block all requests and count all requests for a new policy. 
	- Some of the characteristics are:
		○ Origin IP addresses
		○ Origin Country
		○ Length of the requests
		○ Request Headers
		○ Strings that appears in requests
		○ Presence of malicious SQL code.

# What is DDoS attack and how to minimize
	- Denial of Service is trying to access to service using multiple sessions
	- Tools used are AWS Shield, WAF, Route 53, CloudFront

AWS Leadership principles
	- Customer Obsession
	- Invent & Simplify (Lead teams that innovate and invent)
	- Have backbone; Disagree & commit 9challenge decisions and then commit)
	- Bias for Action (getting things done)
	- Earn Trust
	- Are right, A lot
	- Hire & develop the best
	- Learn and be curious
	- Frugality (Achieve more with less)
	- Think Big
	- Ownership (Take ownership of situations and be responsible & accountable)
	- Dive Deep ( Look into things deeply and analyze data/information)
	- Insists on the highest standard
	- Deliver results.


# What are type of EC2 Instances?
R - Memory Optimized
C- Computer Optimized
R - Memory Optimized
I - Storage Optimized
T - burstable (based on CPU credits and are General Purpose)
G - GPU intensives
M - Medium Optimized

# Explain  CloudFormation function
	- Fn:Join
	- Fn:Select
	- F::FindInMap
	- Fn::Base64
	- Fn::FindInMap
	- Ref

# What are the benefits of the Elastic Beanstalk?
	1- Easy and simple: Elastic Beanstalk enables you to manage and deploy the application easily and quickly.
	2- Autoscaling: Beanstalk scales up or down automatically when your application traffic increases or decreases. 
	3- Developer productivity: Developers can easily deploy the application without any knowledge, but they need to maintain the application securely and user-friendly.
	4- Cost-effective: No charge for Beanstalk. Charges are applied for the AWS service resources which you are using for your application.
	5- Customization: Elastic Beanstalk allows users to select the configurations of AWS services that user want to use them for application development. 
	6- Management and updates: It updates the application automatically when it changes the platform. Platform updates and infrastructure management are taken care of by AWS professionals.

# What are the differences between continuous integration, continuous delivery, and continuous deployment?
- Developers practicing continuous integration merge their changes back to the main branch as often as possible. By doing so, you avoid the integration hell that usually happens when people wait for release day to merge their changes into the release branch.
- Continuous delivery is an extension of continuous integration to make sure that you can release new changes to your customers quickly in a sustainable way. This means that on top of having automated your testing, you also have automated your release process and you can deploy your application at any point of time by clicking on a button.
- continuous deployment goes one step further than continuous delivery. With this practice, every change that passes all stages of your production pipeline is released to your customers. There's no human intervention, and only a failed test will prevent a new change to be deployed to production.

# Situations:

When did you failed in current job and how did you cope up?
-------------------------------------------------------------------------------
- S While working on the Auto Renewal project Business made a call to accept the autorenewal data at stores from customer even 10 months before we started the implementation
- T Now in last 10 months we had 100+ million orders sitting in s3 folder. During the implementation we analyzed the store data and found that stores were not taking the Billing zip State and Billing year which was mandatory with the Zuora system which was our subscription platform
- A While the team was working on the implementation I decided to fork out the from the architecture and build the utility to fix the orders. I worked with another team to come up with the repair utility in which we were wrote AWS crawler to scan through all the 100 million order, put in dynamo DB, which will trigger lambda. Lambda will call the UPS service the fetch the address and ffix the order xml and will drop it to another s3 folder. 
- R This design failed when we tried to run it in production because crawler was not able to handle this. We had to open a ticket with AWS and tried to filter the data for crawler. We had to remove the crawler and use s3 batch to read the data and put in dynamo DB. 

Customer Obsession.
-----------------------------
S - POS team approached with a problem that orders taken at stores are not having Billing ZipCode and CreditCard expiration year which was needed to subscription project.
T - Did a deep dive into the situation and found that all the POS orders were store in s3 bucket, all credit card information was sent to ODS application, more than 100 million orders in s3
A- came up with temporary cloud solution to fix all the 100 millions records in 2 weeks. As per the solution we designed a Crawler which will go through s3 and will filter out certain data and will dump to dynamo, as the row was inserted in dynamo which will trigger the lambda which in turn will call the ups service to get the zip code and ODS system to get the CC billing date and will drop the fixed order xml in another s3 folder. 
R - When we moved the crawler to prod we had issues with the performance and had to tweak filter the monthly data in crawler. The utility was able to process all the 100+ million order on couple of days and we were able to feed the 1 year worth of data to subscription application.

Invent & Simplify example
------------------------------------
S - Gamestop migrated the website to SalesForce and were having the salesforce vendor working on it. Than business came up with the need to let vendor let go and as part that we need to migrate the build process to gitlab to from Jenkins
T - As part if this situation I was tasked to understand the build and deployment process of website and also understand the salesforce architecture to support.
A - We migrated the repository from bitbucket to gitlab without disrupting the existing development. Came up with the gitlab CI/CD deployment process, designed bash scripts which was used to compile the website code in docker container. We also had to open the firewall ports and generate new certificates to make sure the deployment happened.. I also also upgraded the node version 
R - We came up with more robust and automated CI/CD process in gitlab. 

Owner Ship
--------------
S - Couple of weeks back we had issues where the OMS was not able to ingest the orders from the website because some promotions were enabled by business earlier by a day. This  impacting the sales and P1 issue was created. 
T - We analyzed the problem and found that since new promotions were created and hence website was adding multiple promotions in the order.xml in s3 bucket. When OMS was trying to consume the orders they were seeing multiple promotions and was throwing error. So instead of moving away from the situation by saying its OMS issue, I took the ownership and came up with some solution to fix the orders.
A - I created the PowerShell script and used aws cli to download the all the impacted orders from the S3 folder. Once downloaded used the PowerShell script to remove the extra promotions and fixed the orders. Than dropped 18k+ orders(worth 1.1M) back to s3 folder and OMS was able to re-process the orders successfully.
R - It took 3hours to come with the solution which was impacting the customers. But finally management was happy that we were able to mitigate the issue without the revenue loss.

Bias For Action (Getting things done)
-------------------------------------------------
S - Business was reporting that company was loosing 30%-40% buy online and pickup at store orders which was a revenue loss.
T - I was asked to look into this as this was critical bcos of the revenue loss. I broke down this into various task like creating the overall flow document for BOPS, setting up meetings with various parties involved to find out how much time BOPS order takes in each system and how can we fine tune. 
A - I started looking into this and found that BOPS order are touching various system like Website, OMS, Stores System, Radial and found the issue at multiple places like website was dropping the BOPS order in fire and forget to s3 folder and there was no exception handling and then it calls rest api where it was not considering the commit quantity and hence was taking more orders than available qty. I documented the fix for website and then rest api service and also worked with third party vendor Radial to fine tune the bops processing time.
R - As a result the failure rate for BOPS order came from 30%-40% to 3% which was a big win. Also on an average BOPS order was taking around 30 minutes to flow to the order. 

