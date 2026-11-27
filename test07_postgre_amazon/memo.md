
## postgre 설치하고 sample data 적재

```bash
ansible-playbook ec2_bootstrap.yml
ansible-playbook postgre_setup.yml
ansible-playbook scott_setup.yml
```

