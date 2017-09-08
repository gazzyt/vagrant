# Vagrant Samples
This folder contains sample vagrantfiles that I have found useful.

## basic
A basic VM with 4GB memory which sets the hostname and vmname as displayed in HyperV manager.

## dev-vm-with-rdp
A version of the basic vm that installs and configures RDP access to the guest. After 

```PowerShell
vagrant up
```

you will be able to run 

```PowerShell
vagrant rdp
```

and login with the vagrant user.
