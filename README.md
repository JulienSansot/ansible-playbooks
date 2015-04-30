# ansible-playbooks
A collection of Ansible playbooks


aws-cloudwatch
-------
Setup your AWS EC2 instances to send system information (memory, swap, disk space) to CloudWatch (https://console.aws.amazon.com/cloudwatch) every 5 minutes.

You need to :
- Put the IPs of your instances in the hosts files
- Put some proper AWS Access key and secret key in the aws-cloudwatch.yml file

then you can run
```bash
ansible-playbook -i hosts aws-cloudwatch/main.yml
```
