# Requirements:
* virtualbox
* packer
* ansible

# Usage
To build the virtual appliance, run:

```packer build ubuntu1604-microk8s.json```
```packer build centos7.json```

This will generate ovf and vmdk files in output-virtualbox-iso

# Todo
* Better password handling (currently passed as plaintext and it's printed in logs)
* Improve Username Password Configuration (has to be declared in both preseed.cfg and ubuntu1604-microk8s.json)

## Reference links:
* https://github.com/geerlingguy/packer-ubuntu-1604
* builder.boot_commands: https://packer.io/docs/builders/virtualbox-iso.html#boot-command 
* http/preseed.cfg : https://help.ubuntu.com/16.04/installation-guide/amd64/apb.html 
* preseed http server: https://packer.io/docs/builders/virtualbox-iso.html#http_directory https://packer.io/docs/builders/virtualbox-iso.html#templates-inside-boot-command
