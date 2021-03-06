README.md

# Install Ansible

## On local machine (with macOS):

```
sudo easy_install pip
sudo pip install ansible
```

# Prerequisites

1. Boot up an instance of Ubuntu Wily(15.10)
2. Set up DNS record: "A blog.example.com 111.11.11.11"
3. Modify vars section of playbook

# Run script:

`ansible-playbook -i 'serveraddress.com,' setup.yml`
                                       ^ Notice the comma! It is required!

#TODO:
- move variables to separate file
- setup sendmail - http://blog.antoniokov.com/all/blogengine-on-digitalocean/ (ru)
- use tags
- refactor playbook with ansible roles
- SSL config?
- setup sftp

# Misc

## Related LAMP stack installation links:

- https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-16-04
- https://www.digitalocean.com/community/tutorials/how-to-configure-apache-using-ansible-on-ubuntu-14-04
- https://docs.google.com/document/d/14Sb3m9NvNDKMeVF7t9rlhop-S1d_chSNFGbJvnOVe9I/edit#
- http://blog.antoniokov.com/all/blogengine-on-digitalocean/ (ru)

## Not working out of the box but useful playbooks:

- https://github.com/fourkitchens/server-playbooks
- http://labs.qandidate.com/blog/2013/11/21/installing-a-lamp-server-with-ansible-playbooks-and-roles/

## Related ansible links:

- http://docs.ansible.com/ansible/unarchive_module.html
- http://docs.ansible.com/ansible/mysql_db_module.html
- http://docs.ansible.com/ansible/copy_module.html
- http://docs.ansible.com/ansible/file_module.html

## Vsftpd:

- http://serverfault.com/questions/364935/vsftp-login-errors-530-login-incorrect
- https://www.digitalocean.com/community/tutorials/how-to-set-up-vsftpd-on-ubuntu-12-04
