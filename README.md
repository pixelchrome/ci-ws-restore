# Cloud Insights - Workload Security - Restore single or multiple files

## Requirements

### Install Ansible

`sudo apt install ansible`
`ansible-galaxy collection install -r requirements.yml`

### Install python lib `netapp-lib`

`pip3 install netapp-lib`

## Recovery

### Create the CSV file with Workload Security

### Remove the first two Lines from the CSV File

(Something like this below, don't forget the 2nd/blank line)

```csv
"Showing top 100,000 results. Expression: ((protocol:NFS) AND deviceName:*wrk\-svm1* AND (activityType:delete)); TimeRange: [Jul 1 2024 17:16:42 CEST
to Jul 2 2024 17:16:42 CEST]"
```
