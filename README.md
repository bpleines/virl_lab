Automation Practice VIRL Lab

Requirements
------------

<ul>
<li>boto</li>
<li>boto3</li>
<li>botocore</li>
<li>python >= 2.6</li>
</ul>

Role Variables
--------------
Example required configurables to be supplied below in <i>group_vars/all/main.yml</i>:

```yaml
#These values must be configured
vpc_id: vpc-c4c7cda2
vpc_subnet_id: subnet-9e6884b2
region: us-east-1
key_pair: tower_rds
```

Secret Variables are vaulted in group_vars/all/vault.yml
```yaml
---
aws_access_key: ********************
aws_secret_key: ******************************
```

Provision VIRL Infrastructure
-----------------

```
ansible-playbook provision-virl.yml --ask-vault-pass
```

Author Information
------------------
```
Colin McCarthy
Branden Pleines
```
