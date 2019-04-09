
#Add your AWS pem key for ssh access

```
ssh-add YOUR_AWS_KEY.pem 
```

#Use the --check flag first time to check the output

```
ansible-playbook jenkins-ansible.yml --check
```

When running the playbook live you will be given a Jenkins initialse password at the end like this:

```
"passwd:some-random-string-of-chars"
```

Copy all of that without 'passwd:' and then go to the server DNS or ip address with :8080 at the end and login with admin 
and the above copied password. You will then go through the rest of the plugins installation and setup.

Potential issues when trying to install Jenkins plugins via the browser (already handled in the playbook)

https://stackoverflow.com/questions/41055669/unable-to-connect-to-jenkins-server-amazon-linux-ami

https://issues.jenkins-ci.org/browse/JENKINS-45388

If after logging into the GUI you get a blank screen you may need to ssh into the Jenkins server and stop/start the service.


