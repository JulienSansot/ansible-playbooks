# ansible-playbooks
A collection of Ansible playbooks


aws-cloudwatch
-------
To setup your AWS EC2 instances to send system information (memory, swap, disk space) to CloudWatch (https://console.aws.amazon.com/cloudwatch) every 5 minutes.

You need to :
- put the IPS of your instances in the hosts files
- customize some proper of the AWS Access key and secret key in the aws-cloudwatch.yml file

then you can run
```bash
ansible-playbook -i hosts  aws-cloudwatch/main.yml
```
