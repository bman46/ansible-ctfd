# ansible-ctfd
Ansible playbook for deploying [CTFd](https://github.com/CTFd/CTFd)

## How to deploy
* Change ```inventory``` file
* Give it a shot with:
```bash
ansible-playbook -i inventory -e enable_ssl=true site.yml 
```
### SSL
Don't forget to point your A records to server ip
### Notes
Was deployed on top of:
```bash
root@ubuntu-s-1vcpu-1gb-nyc1-01:~# tail /etc/*release
==> /etc/lsb-release <==
DISTRIB_ID=Ubuntu
DISTRIB_RELEASE=20.04
DISTRIB_CODENAME=focal
DISTRIB_DESCRIPTION="Ubuntu 20.04.4 LTS"

==> /etc/os-release <==
ID=ubuntu
ID_LIKE=debian
PRETTY_NAME="Ubuntu 20.04.4 LTS"
VERSION_ID="20.04"
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
VERSION_CODENAME=focal
UBUNTU_CODENAME=focal
```

Happy hacking!
