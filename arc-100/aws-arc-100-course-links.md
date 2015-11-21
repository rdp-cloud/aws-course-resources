```
[course] Architecting on AWS
[course revision] 4.5

[file] aws-arc-100-course-links.md
[file version] 001.001
[file date] 151121

[maintainer] rdepater@amazon.com
```

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

##### [slide] Classless Inter-Domain Routing (CIDR) *

image - CIDR masking - !!!S3 REFERENCE!!! (arc-100-cidrMasking.png)


##### [slide] Subnet Segmentation

image - Subnet Segmentation - !!!S3 REFERENCE!!! (arc-100-subnetSegmentation.png)


##### [slide] VPC Network ACLs Best Practices

doc - NACL Examples - http://docs.aws.amazon.com/AmazonVPC/latest/UserGuide/VPC_Appendix_NACLs.html


##### [slide] Private Network Connection to AWS Cloud

doc - DX Pricing - https://aws.amazon.com/directconnect/pricing/


##### [slide] One VPC or Multiple VPCs?

image - Multi VPC drivers - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/services/vpc/VPC-multiVPCdrivers.png



## Module 03 - Computing in the cloud

##### [slide] Where Does the Operating System Come From?

ref - CloudEndure - https://aws.amazon.com/marketplace/search/results/ref=gtw_navgno_search_box?page=1&searchTerms=cloudendure


##### [slide] Amazon EC2 Instance Type Naming *

image - Instance Naming Convention -  https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/courses/ARC-100/arc-100-instance-naming.png


##### [slide] T2 Instance Type

doc - credit earn/burn rate  - http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/t2-instances.html


##### [slide] Use Case - HA Proxy Under Load *

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

source - https://na32.salesforce.com/06950000001alHV


##### [slide] IOPS and I/O Credits detailed example *

image - GP2 IOPS and I/O credits - https://s3-ap-southeast-2.amazonaws.com/awsedu-assets/courses/ARC-100/arc-100-T2RIgraphic.png

source - salesforce - AWS - an introduction to bursting (GP2 - T2) - https://na32.salesforce.com/sfc/#version/06950000001BsiZ


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

No additional references



## Module 06 - Choosing a datastore

##### [slide] Increasing Performance with Database Caching

whitepaper - Elasticache - https://d0.awsstatic.com/whitepapers/performance-at-scale-with-amazon-elasticache.pdf


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

image - Custom Metric Configuration: Define Metric - !!!S3 REFERENCE!!!  (arc-100-customMetrics-defineMetric.png)

image - Custom Metric Configuration: Define Flows - !!!S3 REFERENCE!!!  (arc-100-customMetrics-defineFlows.png)

image - Custom Metric Configuration: Console Output - !!!S3 REFERENCE!!!  (arc-100-customMetrics-consoleOutput.png)


##### [slide] Store and Monitor Application Log Files with CloudWatch

image - CloudWatch Logs Configuration: Agent Configuration - !!!S3 REFERENCE!!!  (arc-100-cloudwatchLogs-agentConfiguration.png)

image - CloudWatch Logs Configuration: Agent Installation - !!!S3 REFERENCE!!!  (arc-100-cloudwatchLogs-agentInstallation.png)

image - CloudWatch Logs Configuration: Console Output - !!!S3 REFERENCE!!!  (arc-100-cloudwatchLogs-consoleOutput.png)


##### [slide] Cloud Design Pattern: Monitoring Integration Pattern

image - 3rd Party Monitoring: Marketplace - !!!S3 REFERENCE!!!  (arc-100-marketplaceMonitoring.png)


##### [slide] Understanding Elasticity *

image - Understanding Elasticity - !!!S3 REFERENCE!!!  (arc-100-understandingElasticity.png)

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

image - BI Tool integration with RedShift - !!!S3 REFERENCE!!!  (arc-100-redshiftBiIntegration.png)


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

image - Spot is Rewarding - !!!S3 REFERENCE!!!  (arc-100-spotRewards.png)



## Module 13 - HA And DR

##### [slide] Distributed Denial of Service (DDoS) Protection

video - DDoS War Story - https://youtu.be/OT2y3DzMEmQ?t=39m50s


##### [slide] Design for Failure: Basic Principles

blog - Uber: Distributed data across mobile apps -
http://highscalability.com/blog/2015/9/21/uber-goes-unconventional-using-driver-phones-as-a-backup-dat.html

## Global
