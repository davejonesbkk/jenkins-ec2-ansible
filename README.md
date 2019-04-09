
#Add your AWS pem key for ssh access

```
ssh-add YOUR_AWS_KEY.pem 
```

#Use the --check flag first time to check the output

```
ansible-playbook jenkins-ansible.yml --check
```

Potential issues when trying to install Jenkins plugins via the browser (already handled in the playbook)

https://stackoverflow.com/questions/41055669/unable-to-connect-to-jenkins-server-amazon-linux-ami

https://issues.jenkins-ci.org/browse/JENKINS-45388


