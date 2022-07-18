# AWS MySQL Free Tier Playbook

This playbook sets up a MySQL free tier instance.

This is just a labbing playbook to practice ansible with AWS.

The database isn't exposed to the internet. 

Check mode won't work correctly on a first run because there are dependencies in the tasks.

Create var files

./vars/awsconnection.yml

Format

```
aws_id: xxxx
aws_key: xxxx
aws_region: xxxx
task_account: xxxx
```

./vars/mysql.yml

```
username: xxxx
password: xxxx
allocated_storage: xxxx
availability_zone1: xxxx
availability_zone2: xxxx
```

./vars/awsconnection.yml

Install is straight forward

```
ansible-playbook ./install.yml
```

