# gcp-cloudsdk-cheatsheet
This repository contains google cloud shell commands examples

| Name                | Command  | 
| ---                 | ---      | 
| List all instances  | gcloud compute instances list, gcloud compute instance-templates list | 
| Show instance info	| gcloud compute instances describe "<instance-name>" --project "<project-name>" --zone "us-central1-a" |
| Stop an instance	  | gcloud compute instances start --zone=us-central1-a instance-1 |
| Start an instance	  | gcloud compute instances start --zone=us-central1-a instance-1 |
| Create an instance	| gcloud compute instances create vm1 --image image-1 --tags test --zone "<zone>" --machine-type f1-micro |

