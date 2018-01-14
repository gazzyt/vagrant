# vagrant
This project contains sample vagrantfiles for my Vagrant box

# Tips
If you are running vagrant on a domain joined machine then in order for the shared folder to be setup correctly add the following to your Vagrantfile and when prompted for your Windows login enter your userid withou the domain\:
```
config.vm.synced_folder ".", "/vagrant", type: "smb", mount_options: ["domain=mydomain"]
```

If you are using the Lubuntu 1710 box then you also need to set the smb version used (regardless of whether your host is domain joined or not):
```
config.vm.synced_folder ".", "/vagrant", type: "smb", mount_options: ["domain=mydomain","vers=1.0"]
```
