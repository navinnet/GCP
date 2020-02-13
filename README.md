Q1.	You need to ensure reliability for your application and operations by supporting reliable task a scheduling for compute on GCP. Leveraging Google best practices, what should you do?

A. Using the Cron service provided by App Engine, publishing messages directly to a message-processing utility service running on Compute Engine instances.
B. Using the Cron service provided by App Engine, publish messages to a Cloud Pub/Sub topic. Subscribe to that topic using a message-processing utility service running on Compute Engine instances.
C. Using the Cron service provided by Google Kubernetes Engine (GKE), publish messages directly to a message-processing utility service running on Compute Engine instances.
D. Using the Cron service provided by GKE, publish messages to a Cloud Pub/Sub topic. Subscribe to that topic using a message-processing utility service running on Compute Engine instances.

Q2.	You want to enable your running Google Kubernetes Engine cluster to scale as demand for your application changes. What should you do?

A. Add additional nodes to your Kubernetes Engine cluster using the following command:
gcloud container clusters resize
CLUSTER_Name C -size 10
B. Add a tag to the instances in the cluster with the following command:
gcloud compute instances add-tags
INSTANCE – -tags enable­-
autoscaling max-nodes-10
C. Update the existing Kubernetes Engine cluster with the following command:
gcloud alpha container clusters
update mycluster – -enable­
autoscaling – -min-nodes=1 – -max-nodes=10
D. Create a new Kubernetes Engine cluster with the following command:
gcloud alpha container clusters
create mycluster – -enable­-
autoscaling – -min-nodes=1 – -max-nodes=10
and redeploy your application

Q4.	TerramEarth’s CTO wants to use the raw data from connected vehicles to help identify approximately when a vehicle in the field will have a catastrophic failure. You want to allow analysts to centrally query the vehicle data.
Which architecture should you recommend?
A.                                                   B.                                                        

















C.                                                   D.




















Answer: B
Explanation:
The push endpoint can be a load balancer.
A container cluster can be used.
Cloud Pub/Sub for Stream Analytics
 
References:
https://cloud.google.com/pubsub/ https://cloud.google.com/solutions/iot/ https://cloud.google.com/solutions/designing-connected-vehicle-platform https://cloud.google.com/solutions/designing-connected-vehicle-platform#data_ingestion http://www.eweek.com/big-data-and-analytics/google-touts-value-of-cloud-iot-core-for-analyzing­connected-car-data https://cloud.google.com/solutions/iot/

Q5.	Mountkirk Games wants to set up a continuous delivery pipeline. Their architecture includes many small services that they want to be able to update and roll back quickly.
Mountkirk Games has the following requirements:
– Services are deployed redundantly across multiple regions in the US and Europe
– Only frontend services are exposed on the public internet
– They can provide a single frontend IP for their fleet of services
– Deployment artifacts are immutable
Which set of products should they use?
A. Google Cloud Storage, Google Cloud Dataflow, Google Compute Engine
B. Google Cloud Storage, Google App Engine, Google Network Load Balancer
C. Google Kubernetes Registry, Google Container Engine, Google HTTP(S) Load Balancer
D. Google Cloud Functions, Google Cloud Pub/Sub, Google Cloud Deployment Manager

Explanation:

Google Cloud Functions is a serverless environment to build and connect cloud services. Google Cloud Pub/Sub brings the scalability, flexibility, and reliability of enterprise message-oriented middleware to the cloud. By providing many-to-many, asynchronous messaging that decouples senders and receivers, it allows for secure and highly available communication between independently written applications. Google Cloud Pub/Sub delivers low-latency, durable messaging that helps developers quickly integrate systems hosted on the Google Cloud Platform and externally.

Incorrect Answers:
A: Cloud Dataflow is a fully-managed service for transforming and enriching data in stream (real time) and batch (historical) modes.
C: Store your private Docker container images on Cloud Platform for fast, scalable retrieval and deployment. Container Registry is a private Docker repository that works with popular continuous delivery systems. It runs on Cloud Platform to provide consistent uptime on an infrastructure protected by Google’s security. You pay only for storage and internet egress you use, there is no per-image fee.
Reference: https://cloud.google.com/load-balancing/ https://cloud.google.com/solutions/ansible-with-spinnaker-tutorial http://blog.armory.io/what-is-immutable-infrastructure/ https://cloud.google.com/compute/docs/load-balancing/http/

Q8.	For this question, refer to the TerramEarth case study. You need to implement a reliable, scalable GCP solution for the data warehouse for your company, TerramEarth.

Considering the TerramEarth business and technical requirements, what should you do?
A. Replace the existing data warehouse with BigQuery. Use table partitioning.
B. Replace the existing data warehouse with a Compute Engine instance with 96 CPUs.
C. Replace the existing data warehouse with BigQuery. Use federated data sources.
D. Replace the existing data warehouse with a Compute Engine instance with 96 CPUs. Add an additional Compute Engine pre-emptible instance with 32 CPUs.

Q9.	As part of Dress4Win’s plans to migrate to the cloud, they want to be able to set up a managed logging and monitoring system so they can handle spikes in their traffic load.

They want to ensure that:

– The infrastructure can be notified when it needs to scale up and down to handle the ebb and flow of usage throughout the day

– Their administrators are notified automatically when their application reports errors.

– They can filter their aggregated logs down in order to debug one piece of the application across many hosts

Which Google StackDriver features should they use?
A . Logging, Alerts, Insights, Debug
B . Monitoring, Trace, Debug, Logging
C . Monitoring, Logging, Alerts, Error Reporting
D . Monitoring, Logging, Debug, Error Report

Q10.	For this question, refer to the Mountkirk Games case study. You need to analyze and define the technical architecture for the compute workloads for your company, Mountkirk Games. Considering the Mountkirk Games business and technical requirements, what should you do?
A . Create network load balancers. Use preemptible Compute Engine instances.
B . Create network load balancers. Use non-preemptible Compute Engine instances.
C . Create a global load balancer with managed instance groups and autoscaling policies. Use preemptible Compute Engine instances.
D . Create a global load balancer with managed instance groups and autoscaling policies. Use non­preemptible Compute Engine instances.

Q11.	Which is a key requirement for a successful service level agreement?
A . It should be written in legal language
B . It should be simply written and easy to understand
C . It should be based on the service provider’s view of the service
D . It should relate to simple operational metrics

Q12.	For this question, refer to the TerramEarth case study. TerramEarth has decided to store data files in Cloud Storage. You need to configure Cloud Storage lifecycle rule to store 1 year of data and minimize file storage cost.

Which two actions should you take?
A . Create a Cloud Storage lifecycle rule with Age: “30”, Storage Class: “Standard”, and Action: “Set to Coldline”, and create a second GCS life-cycle rule with Age: “365”, Storage Class: “Coldline”, and Action: “Delete”.
B . Create a Cloud Storage lifecycle rule with Age: “30”, Storage Class: “Coldline”, and Action: “Set to Nearline”, and create a second GCS life-cycle rule with Age: “91”, Storage Class: “Coldline”, and Action: “Set to Nearline”.
C . Create a Cloud Storage lifecycle rule with Age: “90”, Storage Class: “Standard”, and Action: “Set to Nearline”, and create a second GCS life-cycle rule with Age: “91”, Storage Class: “Nearline”, and Action: “Set to Coldline”.
D . Create a Cloud Storage lifecycle rule with Age: “30”, Storage Class: “Standard”, and Action: “Set to Coldline”, and create a second GCS life-cycle rule with Age: “365”, Storage Class: “Nearline”, and Action: “Delete”.

Q13.	Dress4Win has asked you to recommend machine types they should deploy their application servers to.

How should you proceed?
A . Perform a mapping of the on-premises physical hardware cores and RAM to the nearest machine types in the cloud.
B . Recommend that Dress4Win deploy application servers to machine types that offer the highest RAM to CPU ratio available.
C . Recommend that Dress4Win deploy into production with the smallest instances available, monitor them over time, and scale the machine type up until the desired performance is reached.
D . Identify the number of virtual cores and RAM associated with the application server virtual machines align them to a custom machine type in the cloud, monitor performance, and scale the machine types up until the desired performance is reached.

Q14.	Dress4Win has asked you for advice on how to migrate their on-premises MySQL deployment to the cloud. They want to minimize downtime and performance impact to their on-premises solution during the migration.

Which approach should you recommend?
A . Create a dump of the on-premises MySQL master server, and then shut it down, upload it to the cloud environment, and load into a new MySQL cluster.
B . Setup a MySQL replica server/slave in the cloud environment, and configure it for asynchronous replication from the MySQL master server on-premises until cutover.
C . Create a new MySQL cluster in the cloud, configure applications to begin writing to both on premises and cloud MySQL masters, and destroy the original cluster at cutover.
D . Create a dump of the MySQL replica server into the cloud environment, load it into: Google Cloud Datastore, and configure applications to read/write to Cloud Datastore at cutover.

Q16.	Mountkirk Games wants to set up a real-time analytics platform for their new game. The new platform must meet their technical requirements.

Which combination of Google technologies will meet all of their requirements?
A . Kubernetes Engine, Cloud Pub/Sub, and Cloud SQL
B . Cloud Dataflow, Cloud Storage, Cloud Pub/Sub, and BigQuery
C . Cloud SQL, Cloud Storage, Cloud Pub/Sub, and Cloud Dataflow
D . Cloud Dataproc, Cloud Pub/Sub, Cloud SQL, and Cloud Dataflow
E . Cloud Pub/Sub, Compute Engine, Cloud Storage, and Cloud Dataproc

Explanation:
Ingest millions of streaming events per second from anywhere in the world with Cloud Pub/Sub, powered by Google’s unique, high-speed private network. Process the streams with Cloud Dataflow to ensure reliable, exactly-once, low-latency data transformation. Stream the transformed data into BigQuery, the cloud-native data warehousing service, for immediate analysis via SQL or popular visualization tools.
From scenario: They plan to deploy the game’s backend on Google Compute Engine so they can capture streaming metrics, run intensive analytics.
Requirements for Game Analytics Platform

Q17.	You want to make a copy of a production Linux virtual machine in the US-Central region. You want to manage and replace the copy easily if there are changes on the production virtual machine. You will deploy the copy as a new instance in a different project in the US-East region.

What steps must you take?
A . Use the Linux dd and netcat commands to copy and stream the root disk contents to a new virtual machine instance in the US-East region.
B . Create a snapshot of the root disk and select the snapshot as the root disk when you create a new virtual machine instance in the US-East region.
C . Create an image file from the root disk with Linux dd command, create a new virtual machine instance in the US-East region
D . Create a snapshot of the root disk, create an image file in Google Cloud Storage from the snapshot, and create a new virtual machine instance in the US-East region using the image file the root disk.

Q18.	Dress4Win would like to become familiar with deploying applications to the cloud by successfully deploying some applications quickly, as is. They have asked for your recommendation.

What should you advise?
A . Identify self-contained applications with external dependencies as a first move to the cloud.
B . Identify enterprise applications with internal dependencies and recommend these as a first move to the cloud.
C . Suggest moving their in-house databases to the cloud and continue serving requests to on-premise applications.
D . Recommend moving their message queuing servers to the cloud and continue handling requests to on-premise applications.

Q19.	TerramEarth’s 20 million vehicles are scattered around the world. Based on the vehicle’s location, its telemetry data is stored in a Google Cloud Storage (GCS) regional bucket (US, Europe, or Asia). The CTO has asked you to run a report on the raw telemetry data to determine why vehicles are breaking down after 100 K miles. You want to run this job on all the data.

What is the most cost-effective way to run this job?
A . Move all the data into 1 zone, then launch a Cloud Dataproc cluster to run the job
B . Move all the data into 1 region, then launch a Google Cloud Dataproc cluster to run the job
C . Launch a cluster in each region to preprocess and compress the raw data, then move the data into a multi-region bucket and use a Dataproc cluster to finish the job
D . Launch a cluster in each region to preprocess and compress the raw data, then move the data into a region bucket and use a Cloud Dataproc cluster to finish the job
Explanation:
Storageguarantees 2 replicates which are geo diverse (100 miles apart) which can get better remote latency and availability.
More importantly, is that multiregional heavily leverages Edge caching and CDNs to provide the content to the end users.
All this redundancy and caching means that Multiregional comes with overhead to sync and ensure consistency between geo-diverse areas. As such, it’s much better for write-once-read-many scenarios. This means frequently accessed (e.g. “hot” objects) around the world, such as website content, streaming videos, gaming or mobile applications.
References: https://medium.com/google-cloud/google-cloud-storage-what-bucket-class-for-the-best­performance-5c847ac8f9f2

Q20.	TerramEarth plans to connect all 20 million vehicles in the field to the cloud. This increases the volume to 20 million 600 byte records a second for 40 TB an hour.

How should you design the data ingestion?
A . Vehicles write data directly to GCS
B . Vehicles write data directly to Google Cloud Pub/Sub
C . Vehicles stream data directly to Google BigQuery
D . Vehicles continue to write data using the existing system (FTP)
Explanation:
Streamed data is available for real-time analysis within a few seconds of the first streaming insertion into a table.
Instead of using a job to load data into BigQuery, you can choose to stream your data into BigQuery one record at a time by using the tabledata().insertAll() method. This approach enables querying data without the delay of running a load job.
References: https://cloud.google.com/bigquery/streaming-data-into-bigquery

Q21.	One of your primary business objectives is being able to trust the data stored in your application. You want to log all changes to the application data.

How can you design your logging system to verify authenticity of your logs?
A . Write the log concurrently in the cloud and on premises
B . Use a SQL database and limit who can modify the log table
C . Digitally sign each timestamp and log entry and store the signature
D . Create a JSON dump of each log entry and store it in Google Cloud Storage

Explanation:
Write a log entry. If the log does not exist, it is created. You can specify a severity for the log entry, and you can write a structured log entry by specifying –payload-type=json and writing your message as a JSON string:
gcloud logging write LOG STRING
gcloud logging write LOG JSON-STRING –payload-type=json
References: https://cloud.google.com/logging/docs/reference/tools/gcloud-logging

Q22.	For this question, refer to the Dress4Win case study. Dress4Win is expected to grow to 10 times its size in 1 year with a corresponding growth in data and traffic that mirrors the existing patterns of usage. The CIO has set the target of migrating production infrastructure to the cloud within the next 6 months.

How will you configure the solution to scale for this growth without making major application changes and still maximize the ROI?
A . Migrate the web application layer to App Engine, and MySQL to Cloud Datastore, and NAS to Cloud Storage. Deploy RabbitMQ, and deploy Hadoop servers using Deployment Manager.
B . Migrate RabbitMQ to Cloud Pub/Sub, Hadoop to BigQuery, and NAS to Compute Engine with Persistent Disk storage. Deploy Tomcat, and deploy Nginx using Deployment Manager.
C . Implement managed instance groups for Tomcat and Nginx. Migrate MySQL to Cloud SQL, RabbitMQ to Cloud Pub/Sub, Hadoop to Cloud Dataproc, and NAS to Compute Engine with Persistent Disk storage.
D . Implement managed instance groups for the Tomcat and Nginx. Migrate MySQL to Cloud SQL, RabbitMQ to Cloud Pub/Sub, Hadoop to Cloud Dataproc, and NAS to Cloud Storage.

Q23.	You are helping the QA team to roll out a new load-testing tool to test the scalability of your primary cloud services that run on Google Compute Engine with Cloud Bigtable.

Which three requirements should they include? Choose 3 answers.
A . Ensure that the load tests validate the performance of Cloud Bigtable
B . Create a separate Google Cloud project to use for the load-testing environment
C . Schedule the load-testing tool to regularly run against the production environment
D . Ensure all third-party systems your services use is capable of handling high load
E . Instrument the production services to record every transaction for replay by the load-testing tool
F . Instrument the load-testing tool and the target services with detailed logging and metrics collection

Q24.	To speed up data retrieval, more vehicles will be upgraded to cellular connections and be able to transmit data to the ETL process. The current FTP process is error-prone and restarts the data transfer from the start of the file when connections fail, which happens often. You want to improve the reliability of the solution and minimize data transfer time on the cellular connections.

What should you do?
A . Use one Google Container Engine cluster of FTP servers. Save the data to a Multi-Regional bucket. Run the ETL process using data in the bucket
B . Use multiple Google Container Engine clusters running FTP servers located in different regions. Save the data to Multi-Regional buckets in US, EU, and Asia. Run the ETL process using the data in the bucket
C . Directly transfer the files to different Google Cloud Multi-Regional Storage bucket locations in US, EU, and Asia using Google APIs over HTTP(S). Run the ETL process using the data in the bucket
D . Directly transfer the files to a different Google Cloud Regional Storage bucket location in US, EU, and Asia using Google APIs over HTTP(S). Run the ETL process to retrieve the data from each Regional bucket
Explanation:
From scenario: They currently have over 500 dealers and service centers in 100 countries.
Multi-Regional Storage is appropriate for storing data that is frequently accessed ("hot" objects), such as serving website content, interactive workloads, or data supporting mobile and gaming applications. Multi-Regional Storage data has the most availability compared to other storage classes.
Multi-Regional Storage is geo-redundant, which means Cloud Storage stores your data redundantly in at least two geographic places separated by at least 100 miles within the multi-regional location of the bucket. Geo-redundancy occurs asynchronously, but Multi-Regional Storage data is redundant within at least one geographic place as soon as you upload it. Like all Cloud Storage data, it is also immediately accessible worldwide.
References: https://cloud.google.com/storage/docs/storage-classes#multi-regional

Q25.	For this question, refer to the Mountkirk Games case study. Mountkirk Games wants you to design a way to test the analytics platform’s resilience to changes in mobile network latency.

What should you do?
A . Deploy failure injection software to the game analytics platform that can inject additional latency to mobile client analytics traffic.
B . Build a test client that can be run from a mobile phone emulator on a Compute Engine virtual machine, and run multiple copies in Google Cloud Platform regions all over the world to generate realistic traffic.
C . Add the ability to introduce a random amount of delay before beginning to process analytics files uploaded from mobile devices.
D . Create an opt-in beta of the game that runs on players’ mobile devices and collects response times from analytics endpoints running in Google Cloud Platform regions all over the world.

Q26.	The current Dress4win system architecture has high latency to some customers because it is located in one data center. As of a future evaluation and optimizing for performance in the cloud, Dresss4win wants to distribute its system architecture to multiple locations when Google cloud platform.

Which approach should they use?
A . Use regional managed instance groups and a global load balancer to increase performance because the regional managed instance group can grow instances in each region separately based on traffic.
B . Use a global load balancer with a set of virtual machines that forward the requests to a closer group of virtual machines managed by your operations team.
C . Use regional managed instance groups and a global load balancer to increase reliability by providing automatic failover between zones in different regions.
D . Use a global load balancer with a set of virtual machines that forward the requests to a closer group of virtual machines as part of a separate managed instance groups.

Q27.	For this question, refer to the Mountkirk Games case study.

Which managed storage option meets Mountkirk’s technical requirement for storing game activity in a time series database service?
A . Cloud Bigtable
B . Cloud Spanner
C . BigQuery
D . Cloud Datastore

Q29.	Your company just finished a rapid lift and shift to Google Compute Engine for your compute needs. You have another 9 months to design and deploy a more cloud-native solution. Specifically, you want a system that is no-ops and auto-scaling.

Which two compute products should you choose? Choose 2 answers.
A . Compute Engine with containers
B . Google Kubernetes Engine with containers
C . Google App Engine Standard Environment
D . Compute Engine with custom instance types
E . Compute Engine with managed instance groups

Explanation:

B: With Container Engine, Google will automatically deploy your cluster for you, update, patch, secure the nodes. Kubernetes Engine’s cluster autoscaler automatically resizes clusters based on the demands of the workloads you want to run.

C: Solutions like Datastore, BigQuery, AppEngine, etc are truly NoOps.

App Engine by default scales the number of instances running up and down to match the load, thus providing consistent performance for your app at all times while minimizing idle instances and thus reducing cost.

Note: At a high level, NoOps means that there is no infrastructure to build out and manage during usage of the platform. Typically, the compromise you make with NoOps is that you lose control of the underlying infrastructure.

References: https://www.quora.com/How-well-does-Google-Container-Engine-support-Google-Cloud­Platform%E2%80%99s-NoOps-claim

Q30.	You want to ensure Dress4Win’s sales and tax records remain available for infrequent viewing by auditors for at least 10 years.

Cost optimization is your top priority.

Which cloud services should you choose?
A . Google Cloud Storage Coldline to store the data, and gsutil to access the data.
B . Google Cloud Storage Nearline to store the data, and gsutil to access the data.
C . Google Bigtabte with US or EU as location to store the data, and gcloud to access the data.
D . BigQuery to store the data, and a web server cluster in a managed instance group to access the data. Google Cloud SQL mirrored across two distinct regions to store the data, and a Redis cluster in a managed instance group to access the data.
Explanation:
Reference: https://cloud.google.com/storage/docs/storage-classes

Q31.	TerramEarth has equipped all connected trucks with servers and sensors to collect telemetry data. Next year they want to use the data to train machine learning models. They want to store this data in the cloud while reducing costs.

What should they do?
A . Have the vehicle’s computer compress the data in hourly snapshots, and store it in a Google Cloud Storage (GCS) Nearline bucket
B . Push the telemetry data in real-time to a streaming dataflow job that compresses the data, and store it in Google BigQuery
C . Push the telemetry data in real-time to a streaming dataflow job that compresses the data, and store it in Cloud Bigtable
D . Have the vehicle’s computer compress the data in hourly snapshots, and store it in a GCS Coldline bucket

Explanation:

Storage is the best choice for data that you plan to access at most once a year, due to its slightly lower availability, 90-day minimum storage duration, costs for data access, and higher per-operation costs.
For example: Cold Data Storage – Infrequently accessed data, such as data stored for legal or regulatory reasons, can be stored at low cost as Coldline Storage, and be available when you need it.
Disaster recovery – In the event of a disaster recovery event, recovery time is key. Cloud Storage provides low latency access to data stored as Coldline Storage.
References: https://cloud.google.com/storage/docs/storage-classes

Q32.	A lead software engineer tells you that his new application design uses websockets and HTTP sessions that are not distributed across the web servers. You want to help him ensure his application will run properly on Google Cloud Platform.

What should you do?
A . Help the engineer to convert his websocket code to use HTTP streaming
B . Review the encryption requirements for websocket connections with the security team
C . Meet with the cloud operations team and the engineer to discuss load balancer options
D . Help the engineer redesign the application to use a distributed user session service that does not rely on websockets and HTTP sessions.
Explanation:
Google Cloud Platform (GCP) HTTP(S) load balancing provides global load balancing for HTTP(S) requests destined for your instances. The HTTP(S) load balancer has native support for the WebSocket protocol.
Incorrect Answers:
A: HTTP server push, also known as HTTP streaming, is a client-server communication pattern that sends information from an HTTP server to a client asynchronously, without a client request. A server push architecture is especially effective for highly interactive web or mobile applications, where one or more clients need to receive continuous information from the server.
References: https://cloud.google.com/compute/docs/load-balancing/http/

Q33.	For this question, refer to the Mountkirk Games case study. You are in charge of the new Game Backend Platform architecture. The game communicates with the backend over a REST API.

You want to follow Google-recommended practices.

How should you design the backend?
A . Create an instance template for the backend. For every region, deploy it on a multi-zone managed instance group. Use an L4 load balancer.
B . Create an instance template for the backend. For every region, deploy it on a single-zone managed instance group. Use an L4 load balancer.
C . Create an instance template for the backend. For every region, deploy it on a multi-zone managed instance group. Use an L7 load balancer.
D . Create an instance template for the backend. For every region, deploy it on a single-zone managed instance group. Use an L7 load balancer.

Q34.	Mountkirk Games wants to set up a real-time analytics platform for their new game. The new platform must meet their technical requirements.

Which combination of Google technologies will meet all of their requirements?
A . Kubernetes Engine, Cloud Pub/Sub, and Cloud SQL
B . Cloud Dataflow, Cloud Storage, Cloud Pub/Sub, and BigQuery
C . Cloud SQL, Cloud Storage, Cloud Pub/Sub, and Cloud Dataflow
D . Cloud Dataproc, Cloud Pub/Sub, Cloud SQL, and Cloud Dataflow
E . Cloud Pub/Sub, Compute Engine, Cloud Storage, and Cloud Dataproc
Explanation:
Ingest millions of streaming events per second from anywhere in the world with Cloud Pub/Sub, powered by Google’s unique, high-speed private network. Process the streams with Cloud Dataflow to ensure reliable, exactly-once, low-latency data transformation. Stream the transformed data into BigQuery, the cloud-native data warehousing service, for immediate analysis via SQL or popular visualization tools.
From scenario: They plan to deploy the game’s backend on Google Compute Engine so they can capture streaming metrics, run intensive analytics.
Requirements for Game Analytics Platform

Q35.	For this question, refer to the Dress4Win case study. Considering the given business requirements, how would you automate the deployment of web and transactional data layers?
A . Deploy Nginx and Tomcat using Cloud Deployment Manager to Compute Engine. Deploy a Cloud SQL server to replace MySQ
B . Deploy Jenkins using Cloud Deployment Manager.
C . Deploy Nginx and Tomcat using Cloud Launcher. Deploy a MySQL server using Cloud Launcher. Deploy Jenkins to Compute Engine using Cloud Deployment Manager scripts.
D . Migrate Nginx and Tomcat to App Engine. Deploy a Cloud Datastore server to replace the MySQL
server in a high-availability configuration. Deploy Jenkins to Compute Engine using Cloud Launcher.
E . Migrate Nginx and Tomcat to App Engine. Deploy a MySQL server using Cloud Launcher. Deploy Jenkins to Compute Engine using Cloud Launcher.

Q36.	For this question, refer to the Dress4Win case study. You are responsible for the security of data stored in Cloud Storage for your company, Dress4Win. You have already created a set of Google Groups and assigned the appropriate users to those groups. You should use Google best practices and implement the simplest design to meet the requirements.

Considering Dress4Win’s business and technical requirements, what should you do?
A . Assign custom IAM roles to the Google Groups you created in order to enforce security requirements. Encrypt data with a customer-supplied encryption key when storing files in Cloud Storage.
B . Assign custom IAM roles to the Google Groups you created in order to enforce security requirements. Enable default storage encryption before storing files in Cloud Storage.
C . Assign predefined IAM roles to the Google Groups you created in order to enforce security requirements. Utilize Google’s default encryption at rest when storing files in Cloud Storage.
D . Assign predefined IAM roles to the Google Groups you created in order to enforce security requirements. Ensure that the default Cloud KMS key is set before storing files in Cloud Storage.

Q37.	Dress4Win has end-to-end tests covering 100% of their endpoints.

They want to ensure that the move to the cloud does not introduce any new bugs.

Which additional testing methods should the developers employ to prevent an outage?
A . They should enable Google Stackdriver Debugger on the application code to show errors in the code.
B . They should add additional unit tests and production scale load tests on their cloud staging environment.
C . They should run the end-to-end tests in the cloud staging environment to determine if the code is working as intended.
D . They should add canary tests so developers can measure how much of an impact the new release causes to latency.

Q37.	A few days after JencoMart migrates the user credentials database to Google Cloud Platform and shuts down the old server, the new database server stops responding to SSH connections. It is still serving database requests to the application servers correctly.

What three steps should you take to diagnose the problem? Choose 3 answers.
A . Delete the virtual machine (VM) and disks and create a new one
B . Delete the instance, attach the disk to a new VM, and investigate
C . Take a snapshot of the disk and connect to a new machine to investigate
D . Check inbound firewall rules for the network the machine is connected to
E . Connect the machine to another network with very simple firewall rules and investigate
F . Print the Serial Console output for the instance for troubleshooting, activate the interactive console, and investigate
Explanation:
D: Handling "Unable to connect on port 22" error message
Possible causes include:
– There is no firewall rule allowing SSH access on the port. SSH access on port 22 is enabled on all Compute Engine instances by default. If you have disabled access, SSH from the Browser will not work. If you run sshd on a port other than 22, you need to enable the access to that port with a custom firewall rule.
– The firewall rule allowing SSH access is enabled, but is not configured to allow connections from GCP Console services. Source IP addresses for browser-based SSH sessions are dynamically allocated by GCP Console and can vary from session to session.
F: Handling "Could not connect, retrying…" error You can verify that the daemon is running by navigating to the serial console output page and looking for output lines prefixed with the accounts-from-metadata: string. If you are using a standard image but you do not see these output prefixes in the serial console output, the daemon might be stopped. Reboot the instance to restart the daemon.
References:
https://cloud.google.com/compute/docs/ssh-in-browser https://cloud.google.com/compute/docs/ssh-in-browser

Q38.	Your customer is moving their corporate applications to Google Cloud Platform. The security team wants detailed visibility of all projects in the organization. You provision the Google Cloud Resource Manager and set up yourself as the org admin.

What Google Cloud Identity and Access Management (Cloud IAM) roles should you give to the security team?
A . Org viewer, project owner
B . Org viewer, project viewer
C . Org admin, project browser
D . Project owner, network admin
References:
A is not correct because Project owner is too broad. The security team does not need to be able to make changes to projects.
B is correct because:
-Org viewer grants the security team permissions to view the organization's display name.
-Project viewer grants the security team permissions to see the resources within projects.
C is not correct because Org admin is too broad. The security team does not need to be able to make changes to the organization.
D is not correct because Project owner is too broad. The security team does not need to be able to make changes to projects.

Q39.	You analyzed TerramEarth’s business requirement to reduce downtime, and found that they can achieve a majority of time saving by reducing customer’s wait time for parts. You decided to focus on reduction of the 3 weeks aggregate reporting time.

Which modifications to the company’s processes should you recommend?
A . Migrate from CSV to binary format, migrate from FTP to SFTP transport, and develop machine learning analysis of metrics
B . Migrate from FTP to streaming transport, migrate from CSV to binary format, and develop machine learning analysis of metrics
C . Increase fleet cellular connectivity to 80%, migrate from FTP to streaming transport, and develop machine learning analysis of metrics
D . Migrate from FTP to SFTP transport, develop machine learning analysis of metrics, and increase dealer local inventory by a fixed factor
Explanation:

The Avro binary format is the preferred format for loading compressed data. Avro data is faster to load because the data can be read in parallel, even when the data blocks are compressed.

Cloud Storage supports streaming transfers with the gsutil tool or boto library, based on HTTP chunked transfer encoding. Streaming data lets you stream data to and from your Cloud Storage account as soon as it becomes available without requiring that the data be first saved to a separate file. Streaming transfers are useful if you have a process that generates data and you do not want to buffer it locally before uploading it, or if you want to send the result from a computational pipeline directly into Cloud Storage.

References: https://cloud.google.com/storage/docs/streaming https://cloud.google.com/bigquery/docs/loading-data

Q40.	The JencoMart security team requires that all Google Cloud Platform infrastructure is deployed using a least privilege model with separation of duties for administration between production and development resources.

What Google domain and project structure should you recommend?
A . Create two G Suite accounts to manage users: one for development/test/staging and one for production. Each account should contain one project for every application
B . Create two G Suite accounts to manage users: one with a single project for all development applications and one with a single project for all production applications
C . Create a single G Suite account to manage users with each stage of each application in its own project
D . Create a single G Suite account to manage users with one project for the development/test/staging environment and one project for the production environment
Explanation:
Note: The principle of least privilege and separation of duties are concepts that, although semantically different, are intrinsically related from the standpoint of security. The intent behind both is to prevent people from having higher privilege levels than they actually need
– Principle of Least Privilege: Users should only have the least amount of privileges required to perform their job and no more. This reduces authorization exploitation by limiting access to resources such as targets, jobs, or monitoring templates for which they are not authorized.
– Separation of Duties: Beyond limiting user privilege level, you also limit user duties, or the specific jobs they can perform. No user should be given responsibility for more than one related function. This limits the ability of a user to perform a malicious action and then cover up that action.
References: https://cloud.google.com/kms/docs/separation-of-duties

Q41.	For this question, refer to the Mountkirk Games case study. Mountkirk Games wants to migrate from their current analytics and statistics reporting model to one that meets their technical requirements on Google Cloud Platform.

Which two steps should be part of their migration plan? (Choose two.)
A . Evaluate the impact of migrating their current batch ETL code to Cloud Dataflow.
B . Write a schema migration plan to denormalize data for better performance in BigQuery.
C . Draw an architecture diagram that shows how to move from a single MySQL database to a MySQL cluster.
D . Load 10 TB of analytics data from a previous game into a Cloud SQL instance, and run test queries against the full dataset to confirm that they complete successfully.
E . Integrate Cloud Armor to defend against possible SQL injection attacks in analytics files uploaded to Cloud Storage.

Q42.	At Dress4Win, an operations engineer wants to create a tow-cost solution to remotely archive copies of database backup files. The database files are compressed tar files stored in their current data center.

How should he proceed?
A . Create a cron script using gsutil to copy the files to a Coldline Storage bucket.
B . Create a cron script using gsutil to copy the files to a Regional Storage bucket.
C . Create a Cloud Storage Transfer Service Job to copy the files to a Coldline Storage bucket.
D . Create a Cloud Storage Transfer Service job to copy the files to a Regional Storage bucket.
Explanation:
Follow these rules of thumb when deciding whether to use gsutil or Storage Transfer Service:
– When transferring data from an on-premises location, use gsutil.
– When transferring data from another cloud storage provider, use Storage Transfer Service.
– Otherwise, evaluate both tools with respect to your specific scenario.
Use this guidance as a starting point.
The specific details of your transfer scenario will also help you determine which tool is more appropriate.

Q43.	Use only fully managed services

CEO Statement

Our last successful game did not scale well with our previous cloud provider, resulting in lower user adoption and affecting the game’s reputation. Our investors want more key performance indicators (KPIs) to evaluate the speed and stability of the game, as well as other metrics that provide deeper insight into usage patterns so we can adapt the game to target users.

CTO Statement

Our current technology stack cannot provide the scale we need, so we want to replace MySQL and move to an environment that provides autoscaling, low latency load balancing, and frees us up from managing physical servers.

CFO Statement

We are not capturing enough user demographic data, usage metrics, and other KPIs. As a result, we do not engage the right users, we are not confident that our marketing is targeting the right users, and we are not selling enough premium Blast-Ups inside the games, which dramatically impacts our revenue.

Mountkirk Games wants you to design their new testing strategy.

How should the test coverage differ from their existing backends on the other platforms?
A . Tests should scale well beyond the prior approaches
B . Unit tests are no longer required, only end-to-end tests
C . Tests should be applied after the release is in the production environment
D . Tests should include directly testing the Google Cloud Platform (GCP) infrastructure
Explanation:
From Scenario:
A few of their games were more popular than expected, and they had problems scaling their application servers, MySQL databases, and analytics tools.
Requirements for Game Analytics Platform include: Dynamically scale up or down based on game activity

Q44.	Your company has decided to make a major revision of their API in order to create better experiences for their developers. They need to keep the old version of the API available and deployable, while allowing new customers and testers to try out the new API. They want to keep the same SSL and DNS records in place to serve both APIs.

What should they do?
A . Configure a new load balancer for the new version of the API
B . Reconfigure old clients to use a new endpoint for the new API
C . Have the old API forward traffic to the new API based on the path
D . Use separate backend pools for each API path behind the load balancer
Explanation:
A is not correct because configuring a new load balancer would require a new or different SSL and DNS records which conflicts with the requirements to keep the same SSL and DNS records.
B is not correct because it goes against the requirements. The company wants to keep the old API available while new customers and testers try the new API.
C is not correct because it is not a requirement to decommission the implementation behind the old API. Moreover, it introduces unnecessary risk in case bugs or incompatibilities are discovered in the new API.
D is correct because an HTTP(S) load balancer can direct traffic reaching a single IP to different backends based on the incoming URL.

Q45.	24 January 2020examsLeave a commentPost navigation
For this question, refer to the Dress4Win case study. To be legally compliant during an audit, Dress4Win must be able to give insights in all administrative actions that modify the configuration or metadata of resources on Google Cloud.

What should you do?
A . Use Stackdriver Trace to create a trace list analysis.
B . Use Stackdriver Monitoring to create a dashboard on the project’s activity.
C . Enable Cloud Identity-Aware Proxy in all projects, and add the group of Administrators as a member.
D . Use the Activity page in the GCP Console and Stackdriver Logging to provide the required insight.

Q46.	For this question, refer to the Dress4Win case study. You want to ensure that your on-premises architecture meets business requirements before you migrate your solution.

What change in the on-premises architecture should you make?
A . Replace RabbitMQ with Google Pub/Sub.
B . Downgrade MySQL to v5.7, which is supported by Cloud SQL for MySQ
C . Resize compute resources to match predefined Compute Engine machine types.
D . Containerize the micro services and host them in Google Kubernetes Engine.

Q47.	The migration of JencoMart’s application to Google Cloud Platform (GCP) is progressing too slowly. The infrastructure is shown in the diagram. You want to maximize throughput.
 
What are three potential bottlenecks? Choose 3 answers.
A . A single VPN tunnel, which limits throughput
B . A tier of Google Cloud Storage that is not suited for this task
C . A copy command that is not suited to operate over long distances
D . Fewer virtual machines (VMs) in GCP than on-premises machines
E . A separate storage layer outside the VMs, which is not suited for this task
F . Complicated internet connectivity between the on-premises infrastructure and GCP

Q48.	Your company runs several databases on a single MySQL instance. They need to take backups of a specific database at regular intervals. The backup activity needs to complete as quickly as possible and cannot be allowed to impact disk performance.

How should you configure the storage?
A . Configure a cron job to use the gcloud tool to take regular backups using persistent disk snapshots.
B . Mount a Local SSD volume as the backup location. After the backup is complete, use gsutil to move the backup to Google Cloud Storage.
C . Use gcsfise to mount a Google Cloud Storage bucket as a volume directly on the instance and write backups to the mounted location using mysqldump.
D . Mount additional persistent disk volumes onto each virtual machine (VM) instance in a RAID10 array and use LVM to create snapshots to send to Cloud Storage
Explanation:
References: https://github.com/mvarrieur/MySQL-backup-to-Google-Cloud-Storage
https://cloud.google.com/storage/docs/gcs-fuse

Q49.	Mountkirk Games wants to set up a real-time analytics platform for their new game. The new platform must meet their technical requirements.

Which combination of Google technologies will meet all of their requirements?
A . Kubernetes Engine, Cloud Pub/Sub, and Cloud SQL
B . Cloud Dataflow, Cloud Storage, Cloud Pub/Sub, and BigQuery
C . Cloud SQL, Cloud Storage, Cloud Pub/Sub, and Cloud Dataflow
D . Cloud Dataproc, Cloud Pub/Sub, Cloud SQL, and Cloud Dataflow
E . Cloud Pub/Sub, Compute Engine, Cloud Storage, and Cloud Dataproc
Explanation:
Ingest millions of streaming events per second from anywhere in the world with Cloud Pub/Sub, powered by Google’s unique, high-speed private network. Process the streams with Cloud Dataflow to ensure reliable, exactly-once, low-latency data transformation. Stream the transformed data into BigQuery, the cloud-native data warehousing service, for immediate analysis via SQL or popular visualization tools.
From scenario: They plan to deploy the game’s backend on Google Compute Engine so they can capture streaming metrics, run intensive analytics.
Requirements for Game Analytics Platform

Q50.	Which of TerramEarth’s legacy enterprise processes will experience significant change as a result of increased Google Cloud Platform adoption?
A . Opex/capex allocation, LAN changes, capacity planning
B . Capacity planning, TCO calculations, opex/capex allocation
C . Capacity planning, utilization measurement, data center expansion
D . Data Center expansion, TCO calculations, utilization measurement

Q51.	JencoMart has decided to migrate user profile storage to Google Cloud Datastore and the application servers to Google Compute Engine (GCE). During the migration, the existing infrastructure will need access to Datastore to upload the data.

What service account key-management strategy should you recommend?
A . Provision service account keys for the on-premises infrastructure and for the GCE virtual machines (VMs)
B . Authenticate the on-premises infrastructure with a user account and provision service account keys for the VMs
C . Provision service account keys for the on-premises infrastructure and use Google Cloud Platform (GCP) managed keys for the VMs
D . Deploy a custom authentication service on GCE/Google Kubernetes Engine (GKE) for the on-premises infrastructure and use GCP managed keys for the VMs
Explanation:
Migrating data to Google Cloud Platform
Let’s say that you have some data processing that happens on another cloud provider and you want to transfer the processed data to Google Cloud Platform. You can use a service account from the virtual machines on the external cloud to push the data to Google Cloud Platform. To do this, you must create and download a service account key when you create the service account and then use that key from the external process to call the Cloud Platform APIs.
References:
https://cloud.google.com/iam/docs/understanding-service­accounts#migrating_data_to_google_cloud_platform

Q52.	Mountkirk Games wants to set up a real-time analytics platform for their new game. The new platform must meet their technical requirements.

Which combination of Google technologies will meet all of their requirements?
A . Kubernetes Engine, Cloud Pub/Sub, and Cloud SQL
B . Cloud Dataflow, Cloud Storage, Cloud Pub/Sub, and BigQuery
C . Cloud SQL, Cloud Storage, Cloud Pub/Sub, and Cloud Dataflow
D . Cloud Dataproc, Cloud Pub/Sub, Cloud SQL, and Cloud Dataflow
E . Cloud Pub/Sub, Compute Engine, Cloud Storage, and Cloud Dataproc
Explanation:
Ingest millions of streaming events per second from anywhere in the world with Cloud Pub/Sub, powered by Google’s unique, high-speed private network. Process the streams with Cloud Dataflow to ensure reliable, exactly-once, low-latency data transformation. Stream the transformed data into BigQuery, the cloud-native data warehousing service, for immediate analysis via SQL or popular visualization tools.

From scenario: They plan to deploy the game’s backend on Google Compute Engine so they can capture streaming metrics, run intensive analytics.

Requirements for Game Analytics Platform

Q53.	For this question, refer to the Mountkirk Games case study. You need to analyze and define the technical architecture for the database workloads for your company, Mountkirk Games.

Considering the business and technical requirements, what should you do?
A . Use Cloud SQL for time series data, and use Cloud Bigtable for historical data queries.
B . Use Cloud SQL to replace MySQL, and use Cloud Spanner for historical data queries.
C . Use Cloud Bigtable to replace MySQL, and use BigQuery for historical data queries.
D . Use Cloud Bigtable for time series data, use Cloud Spanner for transactional data, and use BigQuery for historical data queries.

Q54.	Your company’s test suite is a custom C++ application that runs tests throughout each day on Linux virtual machines. The full test suite takes several hours to complete, running on a limited number of on-premises servers reserved for testing. Your company wants to move the testing infrastructure to the cloud, to reduce the amount of time it takes to fully test a change to the system, while changing the tests as little as possible.

Which cloud infrastructure should you recommend?
A . Google Compute Engine unmanaged instance groups and Network Load Balancer
B . Google Compute Engine managed instance groups with auto-scaling
C . Google Cloud Dataproc to run Apache Hadoop jobs to process each test
D . Google App Engine with Google StackDriver for logging
Explanation:
Google Compute Engine enables users to launch virtual machines (VMs) on demand. VMs can be launched from the standard images or custom images created by users.
Managed instance groups offer autoscaling capabilities that allow you to automatically add or remove instances from a managed instance group based on increases or decreases in load. Autoscaling helps your applications gracefully handle increases in traffic and reduces cost when the need for resources is lower.
Incorrect Answers:
B: There is no mention of incoming IP data traffic for the custom C++ applications.
C: Apache Hadoop is not fit for testing C++ applications. Apache Hadoop is an open-source software framework used for distributed storage and processing of datasets of big data using the MapReduce programming model.
D: Google App Engine is intended to be used for web applications. Google App Engine (often referred to as GAE or simply App Engine) is a web framework and cloud computing platform for developing and hosting web applications in Google-managed data centers.
References: https://cloud.google.com/compute/docs/autoscaler/

Q55.	For this question, refer to the TerramEarth case study. To be compliant with European GDPR regulation, TerramEarth is required to delete data generated from its European customers after a period of 36 months when it contains personal data. In the new architecture, this data will be stored in both Cloud Storage and BigQuery.

What should you do?
A . Create a BigQuery table for the European data, and set the table retention period to 36 months. For Cloud Storage, use gsutil to enable lifecycle management using a DELETE action with an Age condition of 36 months.
B . Create a BigQuery table for the European data, and set the table retention period to 36 months. For Cloud Storage, use gsutil to create a SetStorageClass to NONE action when with an Age condition of 36 months.
C . Create a BigQuery time-partitioned table for the European data, and set the partition expiration period to 36 months. For Cloud Storage, use gsutil to enable lifecycle management using a DELETE action with an Age condition of 36 months.
D . Create a BigQuery time-partitioned table for the European data, and set the partition period to 36 months. For Cloud Storage, use gsutil to create a SetStorageClass to NONE action with an Age condition of 36 months.

Q56.	Your marketing department wants to send out a promotional email campaign. The development team wants to minimize direct operation management. They project a wide range of possible customer

responses, from 100 to 500,000 click-through per day. The link leads to a simple website that explains the promotion and collects user information and preferences.

Which infrastructure should you recommend? Choose 2 answers.
A . Use Google App Engine to serve the website and Google Cloud Datastore to store user data.
B . Use a Google Container Engine cluster to serve the website and store data to persistent disk.
C . Use a managed instance group to serve the website and Google Cloud Bigtable to store user data.
D . Use a single Compute Engine virtual machine (VM) to host a web server, backend by Google Cloud SQ
Explanation:
 
References: https://cloud.google.com/storage-options/

Q57.	JencoMart has built a version of their application on Google Cloud Platform that serves traffic to Asia. You want to measure success against their business and technical goals.

Which metrics should you track?
A . Error rates for requests from Asia
B . Latency difference between US and Asia
C . Total visits, error rates, and latency from Asia
D . Total visits and average latency for users from Asia
E . The number of character sets present in the database
Explanation:
From scenario:
Business Requirements include: Expand services into Asia
Technical Requirements include: Decrease latency in Asia

Q58.	A recent audit revealed that a new network was created in your GCP project. In this network, a GCE instance has an SSH port open to the world. You want to discover this network’s origin.

What should you do?
A . Search for Create VM entry in the Stackdriver alerting console
B . Navigate to the Activity page in the Home section. Set category to Data Access and search for Create VM entry
C . In the Logging section of the console, specify GCE Network as the logging section. Search for the Create Insert entry
D . Connect to the GCE instance using project SSH keys. Identify previous logins in system logs, and match these with the project owners list
Explanation:
Incorrect Answers:
A: To use the Stackdriver alerting console we must first set up alerting policies.
B: Data access logs only contain read-only operations.
Audit logs help you determine who did what, where, and when.
Cloud Audit Logging returns two types of logs:
– Admin activity logs
– Data access logs: Contains log entries for operations that perform read-only operations do not modify any data, such as get, list, and aggregated list methods.
Q59.	For this question, refer to the Dress4Win case study.

Which of the compute services should be migrated as Cis and would still be an optimized architecture for performance in the cloud?
A . Web applications deployed using App Engine standard environment
B . RabbitMQ deployed using an unmanaged instance group
C . Hadoop/Spark deployed using Cloud Dataproc Regional in High Availability mode
D . Jenkins, monitoring, bastion hosts, security scanners services deployed on custom machine types

Q60.	For this question, refer to the Mountkirk Games case study. Mountkirk Games wants to design their solution for the future in order to take advantage of cloud and technology improvements as they become available.

Which two steps should they take? (Choose two.)
A . Store as much analytics and game activity data as financially feasible today so it can be used to train machine learning models to predict user behavior in the future.
B . Begin packaging their game backend artifacts in container images and running them on Kubernetes Engine to improve the availability to scale up or down based on game activity.
C . Set up a CI/CD pipeline using Jenkins and Spinnaker to automate canary deployments and improve development velocity.
D . Adopt a schema versioning tool to reduce downtime when adding new game features that require storing additional player data in the database.
E . Implement a weekly rolling maintenance process for the Linux virtual machines so they can apply critical kernel patches and package updates and reduce the risk of 0-day vulnerabilities.

Q61.	17 January 2020examsLeave a commentPost navigation
For this question, refer to the TerramEarth case study. A new architecture that writes all incoming data to BigQuery has been introduced. You notice that the data is dirty, and want to ensure data quality on an automated daily basis while managing cost.

What should you do?
A . Set up a streaming Cloud Dataflow job, receiving data by the ingestion process. Clean the data in a Cloud Dataflow pipeline.
B . Create a Cloud Function that reads data from BigQuery and cleans it. Trigger it. Trigger the Cloud Function from a Compute Engine instance.
C . Create a SQL statement on the data in BigQuery, and save it as a view. Run the view daily, and save the result to a new table.
D . Use Cloud Dataprep and configure the BigQuery tables as the source. Schedule a daily job to clean the data.

Q62.	Your company places a high value on being responsive and meeting customer needs quickly. Their primary business objectives are release speed and agility. You want to reduce the chance of security errors being accidentally introduced.

Which two actions can you take? Choose 2 answers.
A . Ensure every code check-in is peer reviewed by a security SME
B . Use source code security analyzers as part of the CI/CD pipeline
C . Ensure you have stubs to unit test all interfaces between components
D . Enable code signing and a trusted binary repository integrated with your CI/CD pipeline
E . Run a vulnerability security scanner as part of your continuous-integration /continuous-delivery (CI/CD) pipeline

Q63.	For this question, refer to the TerramEarth case study. You are asked to design a new architecture for the ingestion of the data of the 200,000 vehicles that are connected to a cellular network. You want to follow Google-recommended practices.

Considering the technical requirements, which components should you use for the ingestion of the data?
A . Google Kubernetes Engine with an SSL Ingress
B . Cloud IoT Core with public/private key pairs
C . Compute Engine with project-wide SSH keys
D . Compute Engine with specific SSH keys

Q64.	As part of their new application experience, Dress4Wm allows customers to upload images of themselves. The customer has exclusive control over who may view these images.

Customers should be able to upload images with minimal latency and also be shown their images quickly on the main application page when they log in.

Which configuration should Dress4Win use?
A . Store image files in a Google Cloud Storage bucket. Use Google Cloud Datastore to maintain metadata that maps each customer’s ID and their image files.
B . Store image files in a Google Cloud Storage bucket. Add custom metadata to the uploaded images in Cloud Storage that contains the customer’s unique I
D . Use a distributed file system to store customers’ images. As storage needs increase, add more persistent disks and/or nodes. Assign each customer a unique ID, which sets each file’s owner attribute, ensuring privacy of images.
E . Use a distributed file system to store customers’ images. As storage needs increase, add more persistent disks and/or nodes. Use a Google Cloud SQL database to maintain metadata that maps each customer’s ID to their image files.

Q65.	Dress4Win has configured a new uptime check with Google Stackdriver for several of their legacy services. The Stackdriver dashboard is not reporting the services as healthy.

What should they do?
A . Install the Stackdriver agent on all of the legacy web servers.
B . In the Cloud Platform Console download the list of the uptime servers’ IP addresses and create an inbound firewall rule
C . Configure their load balancer to pass through the User-Agent HTTP header when the value matches GoogleStackdriverMonitoring-UptimeChecks (https://cloud.google.com/monitoring)
D . Configure their legacy web servers to allow requests that contain user-Agent HTTP header when the value matches GoogleStackdriverMonitoring-UptimeChecks (https://cloud.google.com/monitoring)

Q66.	For this question, refer to the TerramEarth case study. Considering the technical requirements, how should you reduce the unplanned vehicle downtime in GCP?
A . Use BigQuery as the data warehouse. Connect all vehicles to the network and stream data into BigQuery using Cloud Pub/Sub and Cloud Dataflow. Use Google Data Studio for analysis and reporting.
B . Use BigQuery as the data warehouse. Connect all vehicles to the network and upload gzip files to a Multi-Regional Cloud Storage bucket using gcloud. Use Google Data Studio for analysis and reporting.
C . Use Cloud Dataproc Hive as the data warehouse. Upload gzip files to a MultiRegional Cloud Storage bucket. Upload this data into BigQuery using gcloud. Use Google data Studio for analysis and reporting.
D . Use Cloud Dataproc Hive as the data warehouse. Directly stream data into prtitioned Hive tables. Use Pig scripts to analyze data.

Q67.	The Dress4Win security team has disabled external SSH access into production virtual machines (VMs) on Google Cloud Platform (GCP).

The operations team needs to remotely manage the VMs, build and push Docker containers, and manage Google Cloud Storage objects.

What can they do?
A. Grant the operations engineer access to use Google Cloud Shell.
B. Configure a VPN connection to GCP to allow SSH access to the cloud VMs.
C. Develop a new access request process that grants temporary SSH access to cloud VMs when an operations engineer needs to perform a task.
D. Have the development team build an API service that allows the operations team to execute specific remote procedure calls to accomplish their tasks.

Q68.	Because you do not know every possible future use for the data TerramEarth collects, you have decided to build a system that captures and stores all raw data in case you need it later. How can you most cost-effectively accomplish this goal?

A. Have the vehicles in the field stream the data directly into BigQuery.
B. Have the vehicles in the field pass the data to Cloud Pub/Sub and dump it into a Cloud Dataproc cluster that stores data in Apache Hadoop Distributed File System (HDFS) on persistent disks.
C. Have the vehicles in the field continue to dump data via FTP, adjust the existing Linux machines, and use a collector to upload them into Cloud Dataproc HDFS for storage.
D. Have the vehicles in the field continue to dump data via FTP, and adjust the existing Linux machines to immediately upload it to Cloud Storage with gsutil.
A is not correct because TerramEarth has cellular service for 200,000 vehicles, and each vehicle sends at least one row (120 fields) per second. This exceeds BigQuery's maximum rows per second per project quota[1]. Additionally, there are 20 million total vehicles, most of which perform uploads when connected by a maintenance port, which drastically exceeds the streaming project quota further.

B is not correct because although Cloud Pub/Sub is a fine choice for this application, Cloud Dataproc is probably not. The question posed asks us to optimize for cost. Because Cloud Dataproc is optimized for ephemeral, job-scoped clusters[2], a long-running cluster with large amounts of HDFS storage could be very expensive to build and maintain when compared to managed and specialized storage solutions like Cloud Storage[3].

C is not correct because the question asks us to optimize for cost, and because Cloud Dataproc is optimized for ephemeral, job-scoped clusters[2], a long-running cluster with large amounts of HDFS storage could be very expensive to build and maintain when compared to managed and specialized storage solutions like Cloud Storage[3].

D is correct because several load-balanced Compute Engine VMs would suffice to ingest 9 TB per day, and Cloud Storage is the cheapest per-byte storage offered by Google. Depending on the format, the data could be available via BigQuery immediately, or shortly after running through an ETL job. Thus, this solution meets business and technical requirements while optimizing for cost.

Q69.	Today, TerramEarth maintenance workers receive interactive performance graphs for the last 24 hours (86,400 events) by plugging their maintenance tablets into the vehicle. The support group wants support technicians to view this data remotely to help troubleshoot problems. You want to minimize the latency of graph loads. How should you provide this functionality?

A. Execute queries against data stored in a Cloud SQL.
B. Execute queries against data indexed by vehicle_id.timestamp in Cloud Bigtable.
C. Execute queries against data stored on daily partitioned BigQuery tables.
D. Execute queries against BigQuery with data stored in Cloud Storage via BigQuery federation.
A is not correct because Cloud SQL provides relational database services that are well-suited to OLTP workloads, but not storage and low-latency retrieval of time-series data.

B is correct because Cloud Bigtable is optimized for time-series data. It is cost-efficient, highly available, and low-latency. It scales well. Best of all, it is a managed service that does not require significant operations work to keep running.

C is not correct because BigQuery is fast for wide-range queries, but it is not as well-optimized for narrow-range queries as Cloud Bigtable is. Latency will be an order of magnitude shorter with Cloud Bigtable for this use.

D is not correct because the objective is to minimize latency, and although BigQuery federation offers tremendous flexibility, it doesn't perform as well as native BigQuery storage[2], and will have longer latency than Cloud Bigtable for narrow-range queries.

Q70.	Your agricultural division is experimenting with fully autonomous vehicles. You want your architecture to promote strong security during vehicle operation. Which two architecture characteristics should you consider?

A. Use multiple connectivity subsystems for redundancy.
B. Require IPv6 for connectivity to ensure a secure address space.
C. Enclose the vehicle’s drive electronics in a Faraday cage to isolate chips.
D. Use a functional programming language to isolate code execution cycles.
E. Treat every microservice call between modules on the vehicle as untrusted.
F. Use a Trusted Platform Module (TPM) and verify firmware and binaries on boot.
A is not correct because this improves system durability, but it doesn't have any impact on the security during vehicle operation.
B is not correct because IPv6 doesn't have any impact on the security during vehicle operation, although it improves system scalability and simplicity.
C is not correct because it doesn't have any impact on the security during vehicle operation, although it improves system durability.
D is not correct because merely using a functional programming language doesn't guarantee a more secure level of execution isolation. Any impact on security from this decision would be incidental at best.
E is correct because this improves system security by making it more resistant to hacking, especially through man-in-the-middle attacks between modules.
F is correct because this improves system security by making it more resistant to hacking, especially rootkits or other kinds of corruption by malicious actors.

Q71.	Which of TerramEarth’s legacy enterprise processes will experience significant change as a result of increased Google Cloud Platform adoption?
A. OpEx/CapEx allocation, LAN change management, capacity planning
B. Capacity planning, TCO calculations, OpEx/CapEx allocation
C. Capacity planning, utilization measurement, data center expansion
D. Data center expansion,TCO calculations, utilization measurement
A is not correct because LAN change management processes don't need to change significantly. TerramEarth can easily peer their on-premises LAN with their Google Cloud Platform VPCs, and as devices and subnets move to the cloud, the LAN team's implementation will change, but the change management process doesn't have to.

B is correct because all of these tasks are big changes when moving to the cloud. Capacity planning for cloud is different than for on-premises data centers; TCO calculations are adjusted because TerramEarth is using services, not leasing/buying servers; OpEx/CapEx allocation is adjusted as services are consumed vs. using capital expenditures.
C is not correct because measuring utilization can be done in the same way, often with the same tools (along with some new ones). Data center expansion is not a concern for cloud customers; it is part of the undifferentiated heavy lifting that is taken care of by the cloud provider.
D is not correct because data center expansion is not a concern for cloud customers; it is part of the undifferentiated heavy lifting that is taken care of by the cloud provider. Measuring utilization can be done in the same way, often with the same tools (along with some new ones).

Q72.	You analyzed TerramEarth’s business requirement to reduce downtime and found that they can achieve a majority of time saving by reducing customers’ wait time for parts. You decided to focus on reduction of the 3 weeks’ aggregate reporting time. Which modifications to the company’s processes should you recommend?
A. Migrate from CSV to binary format, migrate from FTP to SFTP transport, and develop machine learning analysis of metrics.
B. Migrate from FTP to streaming transport, migrate from CSV to binary format, and develop machine learning analysis of metrics.
C. Increase fleet cellular connectivity to 80%, migrate from FTP to streaming transport, and develop machine learning analysis of metrics.
D. Migrate from FTP to SFTP transport, develop machine learning analysis of metrics, and increase dealer local inventory by a fixed factor.
A is not correct because machine learning analysis is a good means toward the end of reducing downtime, but shuffling formats and transport doesn't directly help at all.
B is not correct because machine learning analysis is a good means toward the end of reducing downtime, and moving to streaming can improve the freshness of the information in that analysis, but changing the format doesn't directly help at all.
C is correct because using cellular connectivity will greatly improve the freshness of data used for analysis from where it is now, collected when the machines are in for maintenance. Streaming transport instead of periodic FTP will tighten the feedback loop even more. Machine learning is ideal for predictive maintenance workloads.
D is not correct because machine learning analysis is a good means toward the end of reducing downtime, but the rest of these changes don't directly help at all.

Q73.	Your company wants to deploy several microservices to help their system handle elastic loads. Each microservice uses a different version of software libraries. You want to enable their developers to keep their development environment in sync with the various production services. Which technology should you choose?
A. RPM/DEB
B. Containers
C. Chef/Puppet
D. Virtual machines
A is not correct because although OS packages are a convenient way to distribute and deploy libraries, they don't directly help with synchronizing. Even with a common repository, the development environments will probably deviate from production.
B is correct because using containers for development, test, and production deployments abstracts away system OS environments, so that a single host OS image can be used for all environments. Changes that are made during development are captured using a copy-on-write filesystem, and teams can easily publish new versions of the microservices in a repository.
C is not correct because although infrastructure configuration as code can help unify production and test environments, it is very difficult to make all changes during development this way.
D is not correct because virtual machines run their own OS, which will eventually deviate in each environment, just as now.
Q74.	Your company wants to track whether someone is present in a meeting room reserved for a scheduled meeting. There are 1000 meeting rooms across 5 offices on 3 continents. Each room is equipped with a motion sensor that reports its status every second. You want to support the data upload and collection needs of this sensor network. The receiving infrastructure needs to account for the possibility that the devices may have inconsistent connectivity. Which solution should you design?
A. Have each device create a persistent connection to a Compute Engine instance and write messages to a custom application.
B. Have devices poll for connectivity to Cloud SQL and insert the latest messages on a regular interval to a device specific table.
C. Have devices poll for connectivity to Cloud Pub/Sub and publish the latest messages on a regular interval to a shared topic for all devices.
D. Have devices create a persistent connection to an App Engine application fronted by Cloud Endpoints, which ingest messages and write them to Cloud Datastore.
A is not correct because having a persistent connection does not handle the case where the device is disconnected.
B is not correct because Cloud SQL is a relational database and not the best fit for sensor data. Additionally, the frequency of the writes has the potential to exceed the supported number of concurrent connections.
C is correct because Cloud Pub/Sub can handle the frequency of this data, and consumers of the data can pull from the shared topic for further processing.
D is not correct because having a persistent connection does not handle the case where the device is disconnected.

Q75.	Your company wants to try out the cloud with low risk. They want to archive approximately 100 TB of their log data to the cloud and test the analytics features available to them there, while also retaining that data as a long-term disaster recovery backup. Which two steps should they take?
A. Load logs into BigQuery.
B. Load logs into Cloud SQL.
C. Import logs into Stackdriver.
D. Insert logs into Cloud Bigtable.
E. Upload log files into Cloud Storage.
A is correct because BigQuery is the fully managed cloud data warehouse for analytics and supports the analytics requirement.
B is not correct because Cloud SQL does not support the expected 100 TB. Additionally, Cloud SQL is a relational database and not the best fit for time-series log data formats.
C is not correct because Stackdriver is optimized for monitoring, error reporting, and debugging instead of analytics queries.
D is not correct because Cloud Bigtable is optimized for read-write latency and analytics throughput, not analytics querying and reporting.
E is correct because Cloud Storage provides the Coldline storage class to support long-term storage with infrequent access, which would support the long-term disaster recovery backup requirement.

Q76.	You set up an autoscaling instance group to serve web traffic for an upcoming launch. After configuring the instance group as a backend service to an HTTP(S) load balancer, you notice that virtual machine (VM) instances are being terminated and re-launched every minute. The instances do not have a public IP address. You have verified that the appropriate web response is coming from each instance using the curl command. You want to ensure that the backend is configured correctly. What should you do?
A. Ensure that a firewall rule exists to allow source traffic on HTTP/HTTPS to reach the load balancer.
B. Assign a public IP to each instance, and configure a firewall rule to allow the load balancer to reach the instance public IP.
C. Ensure that a firewall rule exists to allow load balancer health checks to reach the instances in the instance group.
D. Create a tag on each instance with the name of the load balancer. Configure a firewall rule with the name of the load balancer as the source and the instance tag as the destination.
A is not correct because the issue to resolve is the VMs being terminated, not access to the load balancer.
B is not correct because this introduces a security vulnerability without addressing the primary concern of the VM termination.
C is correct because health check failures lead to a VM being marked unhealthy and can result in termination if the health check continues to fail. Because you have already verified that the instances are functioning properly, the next step would be to determine why the health check is continuously failing.
D is not correct because the source of the firewall rule that allows load balancer and health check access to instances is defined IP ranges, and not a named load balancer. Tagging the instances for the purpose of firewall rules is appropriate but would probably be a descriptor of the application, and not the load balancer.

Q77.	Your organization has a 3-tier web application deployed in the same network on Google Cloud Platform. Each tier (web, API, and database) scales independently of the others. Network traffic should flow through the web to the API tier, and then on to the database tier. Traffic should not flow between the web and the database tier. How should you configure the network?
A. Add each tier to a different subnetwork.
B. Set up software-based firewalls on individual VMs.
C. Add tags to each tier and set up routes to allow the desired traffic flow.
D. Add tags to each tier and set up firewall rules to allow the desired traffic flow.
A is not correct because the subnetwork alone will not allow and restrict traffic as required without firewall rules.
B is not correct because this adds complexity to the architecture and the instance configuration.
C is not correct because routes still require firewall rules to allow traffic as requests. Additionally, the tags are used for defining the instances the route applies to, and not for identifying the next hop. The next hop is either an IP range or instance name, but in the proposed solution the tiers are only identified by tags.
D is correct because as instances scale, they will all have the same tag to identify the tier. These tags can then be leveraged in firewall rules to allow and restrict traffic as required, because tags can be used for both the target and source.

Q78.	Your organization has 5 TB of private data on premises. You need to migrate the data to Cloud Storage. You want to maximize the data transfer speed. How should you migrate the data?
A. Use gsutil.
B. Use gcloud.
C. Use GCS REST API.
D. Use Storage Transfer Service.
A is correct because gsutil gives you access to write data to Cloud Storage.
B is not correct because gcloud is the command-line interface for common platform tasks and does not include accessing Cloud Storage.
C is not correct because the data size would require a resumable upload, and that does not meet the requirement of maximizing the data transfer speed.
D is not correct because Storage Transfer Service is for importing online data, not on-premises. Your data source can be an Amazon Simple Storage Service (Amazon S3) bucket, an HTTP/HTTPS location, or a Cloud Storage bucket.

Q79.	You are designing a mobile chat application. You want to ensure that people cannot spoof chat messages by proving that a message was sent by a specific user. What should you do?
A. Encrypt the message client-side using block-based encryption with a shared key.
B. Tag messages client-side with the originating user identifier and the destination user.
C. Use a trusted certificate authority to enable SSL connectivity between the client application and the server.
D. Use public key infrastructure (PKI) to encrypt the message client-side using the originating user’s private key.
A is not correct because although this would encrypt the message, it does not validate either the client or the server.
B is not correct because a malicious actor could spoof the user identifier and destination user information.
C is not correct because SSL only requires the server to have a signed certificate and does not require validating the client.
D is correct because PKI requires that both the server and the client have signed certificates, validating both the client and the server.

Q80.	You are designing a large distributed application with 30 microservices. Each of your distributed microservices needs to connect to a database backend. You want to store the credentials securely. Where should you store the credentials?
A. In the source code
B. In an environment variable
C. In a key management system
D. In a config file that has restricted access through ACLs

A is not correct because storing credentials in source code and source control is discoverable, in plain text, by anyone with access to the source code. This also introduces the requirement to update code and do a deployment each time the credentials are rotated.
B is not correct because consistently populating environment variables would require the credentials to be available, in plain text, when the session is started.
C is correct because key management systems generate, use, rotate, encrypt, and destroy cryptographic keys and manage permissions to those keys.
D is not correct because instead of managing access to the config file and updating manually as keys are rotated, it would be better to leverage a key management system. Additionally, there is increased risk if the config file contains the credentials in plain text.

Q81.	Mountkirk Games wants to set up a real-time analytics platform for their new game. The new platform must meet their technical requirements. Which combination of Google technologies will meet all of their requirements?
A. Kubernetes Engine, Cloud Pub/Sub, and Cloud SQL
B. Cloud Dataflow, Cloud Storage, Cloud Pub/Sub, and BigQuery
C. Cloud SQL, Cloud Storage, Cloud Pub/Sub, and Cloud Dataflow
D. Cloud Pub/Sub, Compute Engine, Cloud Storage, and Cloud Dataproc

A is not correct because Cloud SQL is the only storage listed, is limited to 10 TB of storage, and is better suited for transactional workloads. Mountkirk Games needs queries to access at least 10 TB of historical data for analytic purposes.
B is correct because:
-Cloud Dataflow dynamically scales up or down, can process data in real time, and is ideal for processing data that arrives late using Beam windows and triggers.
-Cloud Storage can be the landing space for files that are regularly uploaded by users’ mobile devices.
-Cloud Pub/Sub can ingest the streaming data from the mobile users.
BigQuery can query more than 10 TB of historical data.
C is not correct because Cloud SQL is the only storage listed, is limited to 10TB of storage, and is better suited for transactional workloads. Mountkirk Games needs queries to access at least 10 TB of historical data for analytic purposes.
D is not correct because Mountkirk Games needs the ability to query historical data. While this might be possible using workarounds, such as BigQuery federated queries for Cloud Storage or Hive queries for Cloud Dataproc, these approaches are more complex. BigQuery is a simpler and more flexible product that fulfills those requirements.

Q82.	Mountkirk Games has deployed their new backend on Google Cloud Platform (GCP). You want to create a thorough testing process for new versions of the backend before they are released to the public. You want the testing environment to scale in an economical way. How should you design the process?
A. Create a scalable environment in GCP for simulating production load.
B. Use the existing infrastructure to test the GCP-based backend at scale.
C. Build stress tests into each component of your application and use resources from the already deployed production backend to simulate load.
D. Create a set of static environments in GCP to test different levels of load—for example, high, medium, and low.
A is correct because simulating production load in GCP can scale in an economical way.
B is not correct because one of the pain points about the existing infrastructure was precisely that the environment did not scale well.
C is not correct because it is a best practice to have a clear separation between test and production environments. Generating test load should not be done from a production environment.
D is not correct because Mountkirk Games wants the testing environment to scale as needed. Defining several static environments for specific levels of load goes against this requirement.

Q83.	Mountkirk Games wants to set up a continuous delivery pipeline. Their architecture includes many small services that they want to be able to update and roll back quickly. Mountkirk Games has the following requirements:
✑ Services are deployed redundantly across multiple regions in the US and Europe
✑ Only frontend services are exposed on the public internet
✑ They can provide a single frontend IP for their fleet of services
✑ Deployment artifacts are immutable
Which set of products should they use?

A. Google Cloud Storage, Google Cloud Dataflow, Google Compute Engine
B. Google Cloud Storage, Google App Engine, Google Network Load Balancer
C. Google Kubernetes Registry, Google Container Engine, Google HTTP(S) Load Balancer
D. Google Cloud Functions, Google Cloud Pub/Sub, Google Cloud Deployment Manager
A is not correct because Mountkirk Games wants to set up a continuous delivery pipeline, not a data processing pipeline. Cloud Dataflow is a fully managed service for creating data processing pipelines.
B is not correct because a Cloud Load Balancer distributes traffic to Compute Engine instances. App Engine and Cloud Load Balancer are parts of different solutions.
C is correct because:
-Google Kubernetes Engine is ideal for deploying small services that can be updated and rolled back quickly. It is a best practice to manage services using immutable containers.
-Cloud Load Balancing supports globally distributed services across multiple regions. It provides a single global IP address that can be used in DNS records. Using URL Maps, the requests can be routed to only the services that Mountkirk wants to expose.
-Container Registry is a single place for a team to manage Docker images for the services.
D is not correct because you cannot reserve a single frontend IP for cloud functions. When deployed, an HTTP-triggered cloud function creates an endpoint with an automatically assigned IP.

Q84.	To reduce costs, the Director of Engineering has required all developers to move their development infrastructure resources from on-premises virtual machines (VMs) to Google Cloud Platform. These resources go through multiple start/stop events during the day and require state to persist. You have been asked to design the process of running a development environment in Google Cloud while providing cost visibility to the finance department. Which two steps should you take?
A. Use persistent disks to store the state. Start and stop the VM as needed.
B. Use the --auto-delete flag on all persistent disks before stopping the VM.
C. Apply VM CPU utilization label and include it in the BigQuery billing export.
D. Use BigQuery billing export and labels to relate cost to groups.
E. Store all state in local SSD, snapshot the persistent disks, and terminate the VM.
F. Store all state in Cloud Storage, snapshot the persistent disks, and terminate the VM.
A is correct because persistent disks will not be deleted when an instance is stopped.
B is not correct because the --auto-delete flag has no effect unless the instance is deleted. Stopping an instance does not delete the instance or the attached persistent disks.
C is not correct because labels are used to organize instances, not to monitor metrics.
D is correct because exporting daily usage and cost estimates automatically throughout the day to a BigQuery dataset is a good way of providing visibility to the finance department. Labels can then be used to group the costs based on team or cost center.
E is not correct because the state stored in local SSDs will be lost when the instance is stopped.
F is not correct because there is no need for persistent disks or snapshots if the state is to be stored in Cloud Storage.

Q85.	The database administration team has asked you to help them improve the performance of their new database server running on Compute Engine. The database is used for importing and normalizing the company’s performance statistics. It is built with MySQL running on Debian Linux. They have an n1-standard-8 virtual machine with 80 GB of SSD zonal persistent disk. What should they change to get better performance from this system in a cost-effective manner?
A. Increase the virtual machine’s memory to 64 GB.
B. Create a new virtual machine running PostgreSQL.
C. Dynamically resize the SSD persistent disk to 500 GB.
D. Migrate their performance metrics warehouse to BigQuery.
 
A is not correct because increasing the memory size will not improve persistent disk throughput.
B is not correct because the DB administration team is requesting help with their MySQL instance. Migration to a different product should not be the solution when other optimization techniques can still be applied first.
C is correct because persistent disk performance is based on the total persistent disk capacity attached to an instance and the number of vCPUs that the instance has. Incrementing the persistent disk capacity will increment its throughput and IOPS, which in turn improve the performance of MySQL.
D is not correct because the DB administration team is requesting help with their MySQL instance. Migration to a different product should not be the solution when other optimization techniques can still be applied first.

Q86.	Mountkirk Games needs to create a repeatable and configurable mechanism for deploying isolated application environments. Developers and testers can access each other’s environments and resources, but they cannot access staging or production resources. The staging environment needs access to some services from production.
What should you do to isolate development environments from staging and production?

A. Create a project for development and test and another for staging and production
B. Create a network for development and test and another for staging and production
C. Create one subnetwork for development and another for staging and production
D. Create one project for development, a second for staging and a third for production
References: https://cloud.google.com/appengine/docs/standard/go/creating-separate-dev-environments

Q87.	For this question, refer to the TerramEarth case study. Considering the technical requirements, how should you reduce the unplanned vehicle downtime in GCP?

A. Use BigQuery as the data warehouse. Connect all vehicles to the network and stream data into BigQuery using Cloud Pub/Sub and Cloud Dataflow. Use Google Data Studio for analysis and reporting.
B. Use BigQuery as the data warehouse. Connect all vehicles to the network and upload gzip files to a Multi-Regional Cloud Storage bucket using gcloud. Use Google Data Studio for analysis and reporting.
C. Use Cloud Dataproc Hive as the data warehouse. Upload gzip files to a MultiRegional Cloud Storage bucket. Upload this data into BigQuery using gcloud. Use Google data Studio for analysis and reporting.
D. Use Cloud Dataproc Hive as the data warehouse. Directly stream data into prtitioned Hive tables. Use Pig scripts to analyze data.


Q5.	JencoMart wants to move their User Profiles database to Google Cloud Platform.
Which Google Database should they use?
A. Cloud Spanner
B. Google BigQuery
C. Google Cloud SQL
D. Google Cloud Datastore

Explanation:
Common workloads for Google Cloud Datastore:
– User profiles
– Product catalogs
– Game state
References: https://cloud.google.com/storage-options/
https://cloud.google.com/datastore/docs/concepts/overview

Q3.	Your development team has created a structured API to retrieve vehicle data. They want to allow third parties to develop tools for dealerships that use this vehicle event data. You want to support delegated authorization against this data. What should you do?

A. Build or leverage an OAuth-compatible access control system
B. Build SAML 2.0 SSO compatibility into your authentication system
C. Restrict data access based on the source IP address of the partner systems
D. Create secondary credentials for each dealer that can be given to the trusted third party

Explanation:
Delegate application authorization with OAuth2
Cloud Platform APIs support OAuth 2.0, and scopes provide granular authorization over the methods that are supported. Cloud Platform supports both service-account and user-account OAuth, also called three-legged OAuth.
References:https://cloud.google.com/docs/enterprise/best-practices-for-enterprise­organizations#delegate_application_authorization_with_oauth2
https://cloud.google.com/appengine/docs/flexible/go/authorizing-apps

Q.	Operational parameters such as oil pressure are adjustable on each of TerramEarth’s vehicles to increase their efficiency, depending on their environmental conditions. Your primary goal is to increase the operating efficiency of all 20 million cellular and unconnected vehicles in the field.
How can you accomplish this goal?
A. Have you engineers inspect the data for patterns, and then create an algorithm with rules that make operational adjustments automatically
B. Capture all operating data, train machine learning models that identify ideal operations, and run locally to make operational adjustments automatically
C. Implement a Google Cloud Dataflow streaming job with a sliding window, and use Google Cloud Messaging (GCM) to make operational adjustments automatically
D. Capture all operating data, train machine learning models that identify ideal operations, and host in Google Cloud Machine Learning (ML) Platform to make operational adjustments automatically
References: https://cloud.google.com/customers/ocado/

Q.	
