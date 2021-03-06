```
[course] Architecting on AWS
[course revision] 4.6

[file] aws-arc-100-course-links.md
[file version] 001.005
[file date] 160211

[maintainer] rdepater@amazon.com
```
<!-- TOC depthFrom:1 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

	- [Module 01 - Computing in the cloud](#module-01-computing-in-the-cloud)
				- [[slide] Deciding Between Regions](#slide-deciding-between-regions)
				- [[slide] How Do I Access AWS?](#slide-how-do-i-access-aws)
				- [[slide] IAM Best Practices](#slide-iam-best-practices)
				- [[slide] Identity and Access Management (IAM) Roles](#slide-identity-and-access-management-iam-roles)
				- [[slide] Tighten Security with IAM](#slide-tighten-security-with-iam)
				- [[slide] IAM Policies](#slide-iam-policies)
				- [[slide] IAM Policy Example: Deny All Except a Specific Resource](#slide-iam-policy-example-deny-all-except-a-specific-resource)
				- [[slide] Federated Users](#slide-federated-users)
				- [[slide] SSO Federation Using SAML (1 of 3)](#slide-sso-federation-using-saml-1-of-3)
				- [[slide] SSO Federation Using SAML (2 of 3)](#slide-sso-federation-using-saml-2-of-3)
				- [[slide] AWS Directory Service (2 of 2)](#slide-aws-directory-service-2-of-2)
				- [[slide] Use Case: Web Identity Federation](#slide-use-case-web-identity-federation)
	- [Module 02 - Extending On Premises Architecture](#module-02-extending-on-premises-architecture)
				- [[slide] Classless Inter-Domain Routing (CIDR)](#slide-classless-inter-domain-routing-cidr)
				- [[slide] Subnet Segmentation](#slide-subnet-segmentation)
				- [[slide] VPC Network ACLs Best Practices](#slide-vpc-network-acls-best-practices)
				- [[slide] Private Network Connection to AWS Cloud](#slide-private-network-connection-to-aws-cloud)
				- [[slide] One VPC or Multiple VPCs?](#slide-one-vpc-or-multiple-vpcs)
	- [Module 03 - Computing in the cloud](#module-03-computing-in-the-cloud)
				- [[slide] Computing in the AWS Cloud: Amazon Elastic Compute Cloud](#slide-computing-in-the-aws-cloud-amazon-elastic-compute-cloud)
				- [[slide] Where Does the Operating System Come From?](#slide-where-does-the-operating-system-come-from)
				- [[slide] Amazon EC2 Instance Type Naming](#slide-amazon-ec2-instance-type-naming)
				- [[slide] T2 Instance Type](#slide-t2-instance-type)
				- [[slide] Use Case - HA Proxy Under Load](#slide-use-case-ha-proxy-under-load)
				- [[slide] Ephemeral Storage](#slide-ephemeral-storage)
				- [[slide] Instrumenting Amazon EC2 Key Pairs](#slide-instrumenting-amazon-ec2-key-pairs)
				- [[slide] What You Can and Cannot Do with ENI?](#slide-what-you-can-and-cannot-do-with-eni)
				- [[slide] Use Cases: Why Would You Use an ENI?](#slide-use-cases-why-would-you-use-an-eni)
				- [[slide] Amazon EC2 Container Service](#slide-amazon-ec2-container-service)
				- [[slide] Shared Responsibility Security Model](#slide-shared-responsibility-security-model)
	- [Module 04 - Designing Storage Subsystems](#module-04-designing-storage-subsystems)
				- [[slide] When to Use Amazon S3 vs. EBS?](#slide-when-to-use-amazon-s3-vs-ebs)
				- [[slide] Amazon EBS Types](#slide-amazon-ebs-types)
				- [[slide] Costs Associated with Amazon EBS (1 of 2)](#slide-costs-associated-with-amazon-ebs-1-of-2)
				- [[slide] IOPS and I/O Credits detailed example](#slide-iops-and-io-credits-detailed-example)
				- [[slide] Large Pool Block Storage](#slide-large-pool-block-storage)
				- [[slide] Amazon EBS Security](#slide-amazon-ebs-security)
				- [[slide] Benefits of Amazon S3](#slide-benefits-of-amazon-s3)
				- [[slide] Amazon S3 Eventual Consistency](#slide-amazon-s3-eventual-consistency)
				- [[slide] Amazon S3 Best Practices](#slide-amazon-s3-best-practices)
				- [[slide] Amazon Glacier Best Practices](#slide-amazon-glacier-best-practices)
				- [[slide] AWS Key Management Service](#slide-aws-key-management-service)
	- [Module 05 - Distributed Environments](#module-05-distributed-environments)
				- [[slide] Use Case: Multi-Region Failover](#slide-use-case-multi-region-failover)
	- [Module 06 - Choosing a datastore](#module-06-choosing-a-datastore)
				- [[slide] Increasing Performance with Database Caching](#slide-increasing-performance-with-database-caching)
				- [[slide] How Can Amazon ElastiCache Help?](#slide-how-can-amazon-elasticache-help)
				- [[slide] Using Oracle GoldenGate with Amazon RDS](#slide-using-oracle-goldengate-with-amazon-rds)
				- [[slide] DynamoDB Topic](#slide-dynamodb-topic)
				- [[slide] Shifting Functionality to NoSQL](#slide-shifting-functionality-to-nosql)
	- [Module 07 - WebScale Media Hosting](#module-07-webscale-media-hosting)
				- [[slide] What If Your Bucket Is Constantly Under Load? (3 of 3)](#slide-what-if-your-bucket-is-constantly-under-load-3-of-3)
				- [[slide] Origin Access Identity to Restrict Access](#slide-origin-access-identity-to-restrict-access)
	- [Module 08 - Event Driven Scaling](#module-08-event-driven-scaling)
				- [[slide] Monitor AWS Resources with Amazon CloudWatch](#slide-monitor-aws-resources-with-amazon-cloudwatch)
				- [[slide] Store and Monitor Application Log Files with CloudWatch](#slide-store-and-monitor-application-log-files-with-cloudwatch)
				- [[slide] Cloud Design Pattern: Monitoring Integration Pattern](#slide-cloud-design-pattern-monitoring-integration-pattern)
				- [[slide] Understanding Elasticity](#slide-understanding-elasticity)
				- [[slide] Compare Auto Scaling, Do-It-Yourself, and Hybrid](#slide-compare-auto-scaling-do-it-yourself-and-hybrid)
				- [[slide] Scaling Amazon RDS with Database Sharding](#slide-scaling-amazon-rds-with-database-sharding)
				- [[slide] Auto Scaling with Dynamic DynamoDB](#slide-auto-scaling-with-dynamic-dynamodb)
	- [Module 09 - Infrastructure As Code](#module-09-infrastructure-as-code)
				- [[slide] Ways To Work with CloudFormation Templates](#slide-ways-to-work-with-cloudformation-templates)
				- [[slide] AWS CloudFormation FAQs](#slide-aws-cloudformation-faqs)
	- [Module 10 - Orchestrating Batch Processing](#module-10-orchestrating-batch-processing)
				- [[slide] Why choose Amazon Simple Queue Service (SQS)?](#slide-why-choose-amazon-simple-queue-service-sqs)
				- [[slide] Amazon SQS Use Cases](#slide-amazon-sqs-use-cases)
				- [[slide] Use Case: Fan-Out](#slide-use-case-fan-out)
	- [Module 11 - Large Scale Design Patterns](#module-11-large-scale-design-patterns)
				- [[slide] Solving the Problem with Amazon Elastic MapReduce](#slide-solving-the-problem-with-amazon-elastic-mapreduce)
				- [[slide] Build in Business Intelligence with Amazon Redshift](#slide-build-in-business-intelligence-with-amazon-redshift)
				- [[slide] Example Application: Twitter-trends.com Website](#slide-example-application-twitter-trendscom-website)
				- [[slide] Solution: Stream Processing with Amazon Kinesis](#slide-solution-stream-processing-with-amazon-kinesis)
				- [[slide] Use Case: Twitter-trends.com Website](#slide-use-case-twitter-trendscom-website)
	- [Module 12 - Designing for Cost](#module-12-designing-for-cost)
				- [[slide] Proactive Cost Optimization with Trusted Advisor](#slide-proactive-cost-optimization-with-trusted-advisor)
				- [[slide] Cloud Design Pattern: Job Observer Pattern](#slide-cloud-design-pattern-job-observer-pattern)
				- [[slide] Fleet Management](#slide-fleet-management)
				- [[slide] Spot Use Cases](#slide-spot-use-cases)
	- [Module 13 - HA And DR](#module-13-ha-and-dr)
				- [[slide] Distributed Denial of Service (DDoS) Protection](#slide-distributed-denial-of-service-ddos-protection)
				- [[slide] Design for Failure: Basic Principles](#slide-design-for-failure-basic-principles)
	- [Global](#global)

<!-- /TOC -->

## Module 01 - Computing in the cloud

##### [slide] Deciding Between Regions

ref - Region latency - http://cloudping.info

doc - AWS Region Services List - http://aws.amazon.com/about-aws/global-infrastructure/regional-product-services/


##### [slide] How Do I Access AWS?

doc - Example API (EC2) - http://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_Operations.html


##### [slide] IAM Best Practices

doc - MFA devices - http://aws.amazon.com/iam/details/mfa/


##### [slide] Identity and Access Management (IAM) Roles

image - IAM Roles Process Flow - http://docs.aws.amazon.com/IAM/latest/UserGuide/images/roles-usingroletodelegate.png


##### [slide] Tighten Security with IAM

doc - IAM Security Policy: Effect - http://docs.aws.amazon.com/IAM/latest/UserGuide/AccessPolicyLanguage_ElementDescriptions.html#Effect

doc - IAM Security Policy: Action - http://docs.aws.amazon.com/IAM/latest/UserGuide/AccessPolicyLanguage_ElementDescriptions.html#Action

doc - IAM Security Policy: Resource - http://docs.aws.amazon.com/IAM/latest/UserGuide/AccessPolicyLanguage_ElementDescriptions.html#Resource


##### [slide] IAM Policies

doc - IAM Evaluation Example - http://docs.aws.amazon.com/IAM/latest/UserGuide/AccessPolicyLanguage_EvaluationLogic.html


##### [slide] IAM Policy Example: Deny All Except a Specific Resource

doc - IAM Security Policy: NotResource - http://docs.aws.amazon.com/IAM/latest/UserGuide/AccessPolicyLanguage_ElementDescriptions.html#NotResource

doc - IAM Security Policy: Variables - http://docs.aws.amazon.com/IAM/latest/UserGuide/PolicyVariables.html


##### [slide] Federated Users

github - Identity Broker Code Example - http://aws.amazon.com/code/4001165270590826


##### [slide] SSO Federation Using SAML (1 of 3)

whitepaper - 3rd Party Federation Example (OKTA) - https://support.okta.com/servlet/fileField?retURL=/articles/Knowledge_Article/28861996-AWS-SAML-integration-with-Okta&entityId=ka0F0000000AaxCIAS&field=File_Attachment__Body__s


##### [slide] SSO Federation Using SAML (2 of 3)

lab - ADFS Qwiklab - https://run.qwiklabs.com/focuses/preview/1596

blog - Implementing ADFS with AWS - http://blogs.aws.amazon.com/security/post/Tx71TWXXJ3UI14/Enabling-Federation-to-AWS-usingWindows-Active-Directory-ADFS-and-SAML-2-0


##### [slide] AWS Directory Service (2 of 2)

blog - AD Connector details - https://blogs.aws.amazon.com/security/post/Tx2PC3QQDXJKASD/How-to-Connect-Your-On-Premises-Active-Directory-to-AWS-Using-AD-Connector

whitepaper - AD in the Cloud - https://d0.awsstatic.com/whitepapers/Implementing_Active_Directory_Domain_Services_in_the_AWS_Cloud.pdf


##### [slide] Use Case: Web Identity Federation

lab - Web Identity Federation Example - https://web-identity-federation-playground.s3.amazonaws.com/index.html



## Module 02 - Extending On Premises Architecture

##### [slide] Classless Inter-Domain Routing (CIDR)

image - CIDR masking - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/courses/ARC-100/arc-100-cidrMasking.png


##### [slide] Subnet Segmentation

image - Subnet Segmentation - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/courses/ARC-100/arc-100-subnetsegmentation.gif


##### [slide] VPC Network ACLs Best Practices

doc - NACL Examples - http://docs.aws.amazon.com/AmazonVPC/latest/UserGuide/VPC_Appendix_NACLs.html


##### [slide] Private Network Connection to AWS Cloud

doc - DX Pricing - https://aws.amazon.com/directconnect/pricing/


##### [slide] One VPC or Multiple VPCs?

image - Multi VPC drivers - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/services/vpc/VPC-multiVPCdrivers.png



## Module 03 - Computing in the cloud

##### [slide] Computing in the AWS Cloud: Amazon Elastic Compute Cloud

video – Adrian Cockcroft: Netflix is 100 000 cores - https://youtu.be/FbuqMFOSVuw?t=7m25s


##### [slide] Where Does the Operating System Come From?

ref - CloudEndure - https://aws.amazon.com/marketplace/search/results/ref=gtw_navgno_search_box?page=1&searchTerms=cloudendure


##### [slide] Amazon EC2 Instance Type Naming

image - Instance Naming Convention -  https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/courses/ARC-100/arc-100-instance-naming.png


##### [slide] T2 Instance Type

doc - credit earn/burn rate  - http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/t2-instances.html


##### [slide] Use Case - HA Proxy Under Load

blog - HAProxy and a t2.micro under load -  http://hipsterdevblog.com/blog/2014/12/19/how-far-can-you-go-with-haproxy-and-a-t2-dot-micro/


##### [slide] Ephemeral Storage

fun - dilbert - http://dilbert.com/strip/2013-06-05


##### [slide] Instrumenting Amazon EC2 Key Pairs

blog - Join Instances to a Domain - https://aws.amazon.com/blogs/aws/seamlessly-join-ec2-instances-to-a-domain/


##### [slide] What You Can and Cannot Do with ENI?

doc - Create a Management Network - http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-eni.html#AvailableIpPerENI


##### [slide] Use Cases: Why Would You Use an ENI?

image - Management network - http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/images/EC2_ENI_management_network.png


##### [slide] Amazon EC2 Container Service

video - re:Invent Intro to ECS -  https://www.youtube.com/watch?v=LE5uBqNp2Ds&feature=youtu.be&t=1m58s


##### [slide] Shared Responsibility Security Model

video - Intro to Shared Responsibility - https://youtu.be/U632-ND7dKQ?list=PLelz-nsz8IfjfsMMHl_zUwdXZtbn8-Zx9

http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-eni.html



## Module 04 - Designing Storage Subsystems

##### [slide] When to Use Amazon S3 vs. EBS?

faq - S3 - http://aws.amazon.com/s3/faqs/


##### [slide] Amazon EBS Types

doc - EBS Product Details - http://aws.amazon.com/ebs/details/


##### [slide] Costs Associated with Amazon EBS (1 of 2)

image - EBS Credit Drain - http://assets.awsedu.com/services/ec2/EBS-CreditDrain.png


##### [slide] IOPS and I/O Credits detailed example

image - GP2 IOPS and I/O credits - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/courses/ARC-100/arc-100-T2RIgraphic.png


##### [slide] Large Pool Block Storage

image - EBS Cost Example - http://assets.awsedu.com/services/ec2/EBS-StripeSavings.png


##### [slide] Amazon EBS Security

doc – No pre-warming - http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-initialize.html


##### [slide] Benefits of Amazon S3

image - Eventual Consistency Diagram - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/courses/ARC-100/arc-100-eventualConsistency.png


##### [slide] Amazon S3 Eventual Consistency

blog - Eventual Consistency - http://shlomoswidler.com/2009/12/read-after-write-consistency-in-amazon.html


##### [slide] Amazon S3 Best Practices

doc - S3 key partitioning and Performance -  http://docs.aws.amazon.com/AmazonS3/latest/dev/request-rate-perf-considerations.html

blog - Multipart Upload -
https://media.amazonwebservices.com/blog/s3_multipart_upload.png


##### [slide] Amazon Glacier Best Practices

image - Tree Hash Alignment - http://docs.aws.amazon.com/amazonglacier/latest/dev/images/TreeHash-ArchiveWithRanges.png

blog - Ranged retrieval - https://aws.amazon.com/blogs/aws/new-range-retrieval-for-amazon-glacier/


##### [slide] AWS Key Management Service

whitepaper - KMS - https://d0.awsstatic.com/whitepapers/KMS-Cryptographic-Details.pdf



## Module 05 - Distributed Environments

##### [slide] Use Case: Multi-Region Failover

video - Route53 adv config - https://www.youtube.com/watch?v=XXUYbdbCb6Q



## Module 06 - Choosing a datastore

##### [slide] Increasing Performance with Database Caching

whitepaper - Elasticache - https://d0.awsstatic.com/whitepapers/performance-at-scale-with-amazon-elasticache.pdf


##### [slide] How Can Amazon ElastiCache Help?

image - Memcachd vs Redis Architecture - http://static1.squarespace.com/static/52ed9a01e4b01528abba472e/t/53321a7de4b054ff7c3311e8/1395833907659/?format=1500w


##### [slide] Using Oracle GoldenGate with Amazon RDS

whitepaper - Oracle Migration - http://d0.awsstatic.com/whitepapers/strategies-for-migrating-oracle-database-to-aws.pdf


##### [slide] DynamoDB Topic

ref – DynamoDB War Story - http://tales.timehop.com/post/113816730211/one-year-of-dynamodb-at-timehop


##### [slide] Shifting Functionality to NoSQL

doc - Session state providers –

Java - https://github.com/aws/aws-dynamodb-session-tomcat

.Net http://docs.aws.amazon.com/AWSSdkDocsNET/latest/V3/DeveloperGuide/net-dg-dynamodb-session.html

PHP - http://www.sitepoint.com/amazon-dynamodb-store-php-sessions-with-load-balancer-2/



## Module 07 - WebScale Media Hosting

##### [slide] What If Your Bucket Is Constantly Under Load? (3 of 3)

blog - S3 Metadata Index Example with Lambda - http://blogs.aws.amazon.com/bigdata/post/Tx2YRX3Y16CVQFZ/Building-and-Maintaining-an-Amazon-S3-Metadata-Index-without-Servers

github - S3 Metadata Index Example with Lambda - https://github.com/awslabs/aws-big-data-blog/tree/master/aws-blog-s3-index-with-lambda-ddb


##### [slide] Origin Access Identity to Restrict Access

doc - IAM Security Policy: Principal - http://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_elements.html#Principal



## Module 08 - Event Driven Scaling

##### [slide] Monitor AWS Resources with Amazon CloudWatch

image - Custom Metric Configuration: Define Metric - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/courses/ARC-100/arc-100-customMetrics-defineMetric.png

image - Custom Metric Configuration: Define Flows - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/courses/ARC-100/arc-100-customMetrics-defineFlows.png

image - Custom Metric Configuration: Console Output - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/courses/ARC-100/arc-100-customMetrics-consoleOutput.png


##### [slide] Store and Monitor Application Log Files with CloudWatch

image - CloudWatch Logs Configuration: Agent Configuration - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/courses/ARC-100/arc-100-cloudwatchLogs-agentConfiguration.png

image - CloudWatch Logs Configuration: Agent Installation - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/courses/ARC-100/arc-100-cloudwatchLogs-agentInstallation.png

image - CloudWatch Logs Configuration: Console Output - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/courses/ARC-100/arc-100-cloudwatchLogs-consoleOutput.png


##### [slide] Cloud Design Pattern: Monitoring Integration Pattern

image - 3rd Party Monitoring: Marketplace - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/courses/ARC-100/arc-100-marketplaceMonitoring.png


##### [slide] Understanding Elasticity

image - Understanding Elasticity - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/courses/ARC-100/arc-100-understandingElasticity.png

whitepaper - AWS Cloud Best Practices - http://media.amazonwebservices.com/AWS_Cloud_Best_Practices.pdf


##### [slide] Compare Auto Scaling, Do-It-Yourself, and Hybrid

doc - AutoScaling Instance Lifecycle Events - http://docs.aws.amazon.com/AutoScaling/latest/DeveloperGuide/AutoScalingGroupLifecycle.html


##### [slide] Scaling Amazon RDS with Database Sharding

site - MySQL Sharding: Spyder  - http://spiderformysql.com/product.html


##### [slide] Auto Scaling with Dynamic DynamoDB

github - Dynamic DynamoDB - http://dynamic-dynamodb.readthedocs.org/en/latest/index.html



## Module 09 - Infrastructure As Code

##### [slide] Ways To Work with CloudFormation Templates

image - CloudFormation Template Elements - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/services/cloudformation/CloudFormation-templateElements.png


##### [slide] AWS CloudFormation FAQs

doc - Install Chef/Puppet via cloud-init - http://cloudinit.readthedocs.org/en/latest/topics/examples.html#install-and-run-chef-recipes



## Module 10 - Orchestrating Batch Processing

##### [slide] Why choose Amazon Simple Queue Service (SQS)?

video - SQS producers and consumers - https://www.youtube.com/watch?v=zwLC5xmCZUs&t=1464


##### [slide] Amazon SQS Use Cases

site - Priority Queues Pattern - http://en.clouddesignpattern.org/index.php/CDP:Priority_Queue_Pattern

doc - AutoScaling and SQS - http://docs.aws.amazon.com/AutoScaling/latest/DeveloperGuide/as-using-sqs-queue.html


##### [slide] Use Case: Fan-Out

video – SNS fanout - https://www.youtube.com/watch?v=zwLC5xmCZUs#t=1849



## Module 11 - Large Scale Design Patterns

##### [slide] Solving the Problem with Amazon Elastic MapReduce

image – map reduce diagram - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/concepts/mapreduce/MR.png


##### [slide] Build in Business Intelligence with Amazon Redshift

image - BI Tool integration with RedShift - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/courses/ARC-100/arc-100-redshiftBiIntegration.png


##### [slide] Example Application: Twitter-trends.com Website

video - Twitter Trends Kinesis Example -  https://youtu.be/AXAaCG2QUkE?t=2m29s


##### [slide] Solution: Stream Processing with Amazon Kinesis

site - Kinesis/Twitter example: CSIRO - http://wefeel.csiro.au/#/


##### [slide] Use Case: Twitter-trends.com Website

github – Java logs into kinesis - https://github.com/awslabs/kinesis-log4j-appender



## Module 12 - Designing for Cost

##### [slide] Proactive Cost Optimization with Trusted Advisor

doc - Trusted Advisor Heuristics - https://aws.amazon.com/premiumsupport/trustedadvisor/best-practices/


##### [slide] Cloud Design Pattern: Job Observer Pattern

blog - scaling based on queue depth, launching spot FLEETs - https://aws.amazon.com/blogs/compute/dynamic-scaling-with-ec2-spot-fleet/


##### [slide] Fleet Management

image - Fault Tolerance Example - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/concepts/ft/ARC-100-faultTolerance.png


##### [slide] Spot Use Cases

image - Spot is Rewarding - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/courses/ARC-100/arc-100-spotRewards.png



## Module 13 - HA And DR

##### [slide] Distributed Denial of Service (DDoS) Protection

video - DDoS War Story - https://youtu.be/OT2y3DzMEmQ?t=39m50s


##### [slide] Design for Failure: Basic Principles

blog - Uber: Distributed data across mobile apps -
http://highscalability.com/blog/2015/9/21/uber-goes-unconventional-using-driver-phones-as-a-backup-dat.html

## Global
