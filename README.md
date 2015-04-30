# ansible-playbooks
A collection of Ansible playbooks

For each playbook you need to edit the variables and the host file

aws-cloudwatch
-------
Setup your AWS EC2 instances to send system information (memory, swap, disk space) to CloudWatch (https://console.aws.amazon.com/cloudwatch) every 5 minutes.
```
ansible-playbook -i hosts aws-cloudwatch/main.yml
```

mongodb-daily-backup-s3
-------
Setup a cron task which will backup your mongo database to s3 every day.
```
ansible-playbook -i hosts mongodb-daily-backup-s3/main.yml
```

postgres-daily-backup-s3
-------
Setup a cron task which will backup your postgreSQL database to s3 every day.
```
ansible-playbook -i hosts postgres-daily-backup-s3/main.yml
```



