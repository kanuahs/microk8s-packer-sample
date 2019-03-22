Requirements:
* virtualbox
* packer
* ansible


To build the virtual appliance, run:

```packer build ubuntu1604-microk8s.json```

This will generate ovf and vmdk files in output-virtualbox-iso



Reference links:
* builder.boot_commands: https://packer.io/docs/builders/virtualbox-iso.html#boot-command 
* http/preseed.cfg : https://help.ubuntu.com/16.04/installation-guide/amd64/apb.html 
* preseed http server: https://packer.io/docs/builders/virtualbox-iso.html#http_directory https://packer.io/docs/builders/virtualbox-iso.html#templates-inside-boot-command