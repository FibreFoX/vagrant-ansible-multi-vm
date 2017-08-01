# Vagrant setup with multiple VMs and Ansible for provisioning

While creating a local development-setup, I realized that I need to avoid having Ansible and the Virtualbox Guest Additions being installed on my development-VM.

This made me search for a way to have [Ansible](https://www.ansible.com/get-started) installed on a separate VM but created by the same Vagrantfile.

This needs vagrant-vbguest being installed:

```sh
vagrant plugin install vagrant-vbguest
```


To create both VMs, just type `vagrant up` and let the magic happen.