## Usage
1. clone this repo
2. cd into this repo
3. run `docker build -t ubuntu_salt_ssh .`
4. `docker run -itd -v "/host_machine_path/etc/salt":"/etc/salt" -v "/host_machine_path/srv/salt":"/srv/salt" -v "/host_machine_path/srv/pillar":"/srv/pillar" --hostname ubuntu_salt_ssh --name ubuntu_salt_ssh_instance ubuntu_salt_ssh`

## Note
Currently salt-ssh default need support python2, therefore salt-ssh might not work for ubuntu16.04 image out of the box