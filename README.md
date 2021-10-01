# OneCoolThing-BigData
Slide 1
# AWS analytics service are build to handle large amount of data ; scale and automate many manual and time consuming tasks. AWS- powered data lakes , supported by unmatched availability of Amazon Simple Storage Service(S3) can handle the scale , agility and flexibility required to combine different data and analytics approaches.

### AWS is the fastest and most effective place to store and analyze data, quickly extract data insight and is optimized to give best performance, scale and cost for your needs.

### AWS offers built in Analytics services where one can build, train and deploy ML models quickly with Amazon SageMaker- fully managed service that provides tools for every step of ML development lifecycle in one integrated envirinment.


## FACTS about AWS:
1. 10000+ Data lakes which is centralized repositories od data in structured and unstructed format usually Blobs or files. 
2. 3X faster than Apache spark
3. 50% less expensive than Cloud data warehouses
4. 3PB of data storage with Amazon open search service.
SLIDE 2
### Amazon OpenSearch Service makes it easy for you to perform interactive log analytics, real-time application monitoring, website search. OpenSearch is an open source, distributed search and analytics suite derived from Elasticsearch. 
# Features:
### Deployment and management:
1. Setup and configuration:
Getting started with Amazon OpenSearch Service is easy. You can set up and configure your Amazon OpenSearch Service cluster using the AWS Management Console or a single API call through the AWS Command Line Interface (CLI). You can specify the number of instances, instance types, storage options, and modify or delete existing clusters at any time.
In-place upgrades: Amazon OpenSearch Service makes it easy to upgrade your OpenSearch and Elasticsearch clusters (up to version 7.10) to newer versions without any downtime, using in-place version upgrades. In-place upgrades eliminates the hassle of taking a manual snapshot, restoring it to a cluster running the newer version, and updating all your endpoint references.

2. Event monitoring and alerting:
Amazon OpenSearch Service provides built-in event monitoring and alerting, enabling you to monitor the data stored in your cluster and automatically send notifications based on pre-configured thresholds. Built using the OpenSearch alerting plugin, this feature lets you configure and manage alerts using your Kibana or OpenSearch Dashboards interface and the REST API. You can receive notifications via custom webhooks, Slack, Amazon Simple Notification Service (SNS), and Amazon Chime. You can also view cluster health metrics including number of instances, cluster health, searchable documents, CPU, and memory, as well as disk utilization for data and master nodes through Amazon CloudWatch, at no additional charge.

3. Support for multiple query languages:
With Amazon OpenSearch Service, there’s no need for OpenSearch query domain-specific language (DSL) proficiency. Write SQL queries with OpenSearch SQL or use the OpenSearch Piped Processing Language (PPL), a query language that lets you use pipe (|) syntax, to explore, discover, and query your data. OpenSearch Dashboards also includes a SQL and PPL workbench.
Integration with open source tools: Amazon OpenSearch Service offers built-in OpenSearch Dashboards and Kibana (Elasticsearch version 7.10 and previous) and integrates with Logstash, so you can ingest and visualize your data using the open source tools you prefer. Perform trace analytics with Amazon OpenSearch Service’s support for the open source OpenTelemetry standard and continue to use your existing code with direct access to Elasticsearch APIs and plugins such as Kuromoji, Phonetic Analysis, Ingest Processor Attachment, Ingest User Agent Processor, and Mapper Murmur3.
4. Security:
With Amazon OpenSearch Service, you can securely connect your applications to your managed Elasticsearch (version 7.10 and previous) or OpenSearch environment from your Amazon Virtual Private Cloud (VPC) or via the public Internet, configuring network access using VPC security groups or IP-based access policies. You can also securely authenticate users and control access using Amazon Cognito, AWS Identity and Access Management (IAM), or basic authentication with a username and password. Amazon OpenSearch Service leverages the OpenSearch security plugin, enabling you to define granular permissions for indices, documents, or fields. You can also extend Kibana with read-only views and secure multi-tenant support. Amazon OpenSearch Service also supports built-in encryption for data at-rest and in-transit, so you can protect your data when it is stored in your domain or in automated snapshots and transferring between nodes in your domain. Amazon OpenSearch Service is HIPAA-eligible and compliant with PCI DSS, SOC, ISO, and FedRAMP standards, making it easy for you to build applications that meet compliance requirements.

Slide 3:


WORKING:
IMAGE+
- you will build a working web application, served from within your VPC and complete with a logging back end provided by Amazon Elasticsearch Service and with real-time monitoring using Kibana. The application provides a movie search experience across 5,000 movies, powered by Amazon ES and served with Apache httpd and PHP. The logging infrastructure sends the httpd web logs to Amazon ES via Amazon ElastiCache for Redis, which we use to buffer the log lines, and Logstash, which transforms and delivers records to Amazon ES.
- You will deploy an internet gateway to allow traffic to flow to your application via an Application Load Balancer, and a proxy/bastion instance to allow administrative and Kibana access.
- For the logging infrastructure, we use Filebeat and Logstash on EC2, Amazon ElastiCache for Redis and of course Amazon Elasticsearch Service. Filebeat is a host-based log shipper that remembers its location if interrupted. Logstash collects, transforms and pushes your data to your desired store which in this case is an Amazon Elasticsearch Service Domain. The combination of these items gives a flexible, configurable, private networked option within VPC that will allow you to scale as your volume increases.
