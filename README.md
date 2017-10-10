# vagrant
This project contains sample vagrantfiles for my Vagrant box

# Tips
If you are running vagrant on a domain joined machine then in order for the shared folder to be setup correctly add the following to your Vagrantfile and when prompted for your Windows login enter your userid withou the domain\:
```
config.vm.synced_folder ".", "/vagrant", type: "smb", mount_options: ["domain=mydomain"]
```