# gcp-cloudsdk-cheatsheet
This repository contains google cloud shell commands examples

# gcp compute engine commnad 
| Name                | Command  | 
| ---                 | ---      | 
| List all instances  | gcloud compute instances list, gcloud compute instance-templates list | 
| Show instance info	| gcloud compute instances describe "<instance-name>" --project "<project-name>" --zone "us-central1-a" |
| Stop an instance	  | gcloud compute instances start --zone=us-central1-a instance-1 |
| Start an instance	  | gcloud compute instances start --zone=us-central1-a instance-1 |
| Create an instance	| gcloud compute instances create vm1 --image image-1 --tags test --zone "<zone>" --machine-type f1-micro |

# gcp disk command

| Name                | Command  | 
| ---                 | ---      | 
| List all disks	  | gcloud compute disks list |
| List all disk types |	gcloud compute disk-types list |
| List all snapshots  |	gcloud compute snapshots list |
| Create snapshot	  | gcloud compute disks snapshot <diskname> --snapshotname <name1> --zone $zone |

# gcp bucket commands 

| Name                | Command  | 
| ---                 | ---      |
| List all buckets and files | gsutil ls, gsutil ls -lh gs://<bucket-name> |
| Download file				 | gsutil cp gs://<bucket-name>/<dir-path>/package-1.1.tgz |
| Upload file	 			 | gsutil cp <filename> gs://<bucket-name>/<directory>/ |
| Cat file					 | gsutil cat gs://<bucket-name>/<filepath>/ |
| Delete file				 | gsutil rm gs://<bucket-name>/<filepath> |
| Move file	                 | gsutil mv <src-filepath> gs://<bucket-name>/<directory>/<dest-filepath> |
| Copy folder                | gsutil cp -r ./conf gs://<bucket-name>/ |
| Show disk usage            | gsutil du -h gs://<bucket-name/<directory> | 
| Create bucket         	 | gsutil mb gs://<bucket-name> |
| Caculate file              | sha1sum	gsha1sum syslog-migration-10.0.2.tgz, shasum syslog-migration-10.0.2.tgz |
| Gsutil help	             | gsutil help, gsutil help cp, gsutil help options |
  
  
  google cloud data engineering - foundational concepts 


1. Which of these are valid Storage services in the data lifecycle? (Choose all that apply)

A - BigQuery
B - Cloud Pub/Sub
C - Cloud Storage
D - Cloud Dataflow
E - Cloud Datastore
F - Data Studio

Correct Answer: ACE

2. You need to deploy a database that will be managed manually on Compute Engine. This database does not need strong transactional consistency or ACID compliance. It does need to support high throughput read/write and must scale to over 20 TB. Choose three possible database options for this task.

A Cassandra
B Oracle
C MySQL
D Microsoft SQL Server
E MongoDB
F HBase

Correct Answer: AEF


3. You are working toward becoming more familiar with the data lifecycle on Google Cloud. Choose which Google Cloud services, in the right order, are involved in the following handling of data:
1.Streaming Data Ingest
2.Processing Pipeline
3.Storage in data warehouse

A  1.Pub/Sub - 2. Dataflow - 3. Cloud Storage
B  1.Dataflow - 2. Pub/Sub - 3. BigQuery
C  1.Pub/Sub - 2. Dataflow - 3. BigQuery
D  1.Pub/Sub - 2. Cloud Storage - 3. BigQuery

Correct Answer: C 

4. You need to deploy an unmanaged database using Compute Engine instances. This database must have strong transactional consistency and meet ACID compliance. It will be no larger than 500 GB. It will be used to track customer medical records. Choose all of the possible database options you can use for this request.

A MySQL
B Cassandra
C Microsoft SQL Server
D Bigtable

Correct Answer: AC

5.  You have a large collection of different types of data that you will need to access regularly, which includes unstructured data. You will only need to access it from your office location in London. What type of storage solution should you use? Choose the single answer that fits all above use cases.

A Standard Regional Cloud Storage bucket
B Regional Coldline bucket
C Multi-regional Cloud Storage bucket
D BigQuery

Correct Answer: A 

6. Which of these is an example of streaming data ingest?

A Loading data from Cloud Storage to Cloud ML engine for training machine learning models.
B Importing the contents of a Cloud Storage bucket to BigQuery for analysis
C Traffic sensors streaming data to Cloud Pub/Sub
D Copying data from your on-premises server to Cloud Storage

Correct Answer: C
