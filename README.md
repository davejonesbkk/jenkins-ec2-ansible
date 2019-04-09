
#Add your AWS pem key for ssh access
ssh-add YOUR_AWS_KEY.pem 

#Use the --check flag first time to check the output
ansible-playbook jenkins-ansible.yml --check

