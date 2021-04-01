# [Exam Guide](https://cloud.google.com/certification/guides/data-engineer?hl=zh-tw)

### Requirement:

- Design data processing systems
- Build and operationalize data processing systems
- Operationalize machine learning models
- Ensure solution quality

## Design data processing systems

1. Selecting the appropriate storage technologies. Considerations include:
   - Mapping storage systems to business requirements
   - Data modeling
   - Tradeoffs involving latency, throughput, transactions
   - Distributed systems
   - Schema design
2. Designing data pipelines. Considerations include:
   - Data publishing and visualization (e.g., BigQuery)
   - Batch and streaming data (e.g., Cloud Dataflow, Cloud Dataproc, Apache Beam, Apache Spark and Hadoop ecosystem, Cloud Pub/Sub, Apache Kafka)
   - Online (interactive) vs. batch predictions
   - Job automation and orchestration (e.g., Cloud Composer)
3. Designing a data processing solution. Considerations include:
   - Choice of infrastructure
   - System availability and fault tolerance
   - Use of distributed systems
   - Capacity planning
   - Hybrid cloud and edge computing
   - Architecture options (e.g., message brokers, message queues, middleware, service-oriented architecture, serverless functions)
   - At least once, in-order, and exactly once, etc., event processing
4. Migrating data warehousing and data processing. Considerations include:
   - Awareness of current state and how to migrate a design to a future state
   - Migrating from on-premises to cloud (Data Transfer Service, Transfer Appliance, Cloud Networking)
   - Validating a migration

## Build and operationalize data processing systems

1. Building and operationalizing storage systems. Considerations include:
   - Effective use of managed services (Cloud Bigtable, Cloud Spanner, Cloud SQL, BigQuery, Cloud Storage, Cloud Datastore, Cloud Memorystore)
   - Storage costs and performance
   - Lifecycle management of data
2. Building and operationalizing pipelines. Considerations include:
   - Data cleansing
   - Batch and streaming
   - Transformation
   - Data acquisition and import
   - Integrating with new data sources
3. Building and operationalizing processing infrastructure. Considerations include:
   - Provisioning resources
   - Monitoring pipelines
   - Adjusting pipelines
   - Testing and quality control

## Operationalize machine learning models

Keep blank temporarily.

## Ensure solution quality

1. Designing for security and compliance. Considerations include:
   - Identity and access management (e.g., Cloud IAM)
   - Data security (encryption, key management)
   - Ensuring privacy (e.g., Data Loss Prevention API)
   - Legal compliance (e.g., Health Insurance Portability and Accountability Act (HIPAA), Children's Online Privacy Protection Act (COPPA), FedRAMP, General Data Protection Regulation (GDPR))
2. Ensuring scalability and efficiency. Considerations include:
   - Building and running test suites
   - Pipeline monitoring (e.g., Stackdriver)
   - Assessing, troubleshooting, and improving data representations and data processing infrastructure
   - Resizing and autoscaling resources
3. Ensuring reliability and fidelity. Considerations include:
   - Performing data preparation and quality control (e.g., Cloud Dataprep)
   - Verification and monitoring
   - Planning, executing, and stress testing data recovery (fault tolerance, rerunning failed jobs, performing retrospective re-analysis)
   - Choosing between ACID, idempotent, eventually consistent requirements
4. Ensuring flexibility and portability. Considerations include:
   - Mapping to current and future business requirements
   - Designing for data and application portability (e.g., multi-cloud, data residency requirements)
   - Data staging, cataloging, and discovery

## Ref

[How I Passed the Google Cloud Professional Data Engineer Certification Exam Without the recommended 3-years hands-on experience](https://towardsdatascience.com/passing-the-google-cloud-professional-data-engineer-certification-87da9908b333)