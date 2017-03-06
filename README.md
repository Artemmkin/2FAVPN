### What do I need to change?

Change the path to your private key in ansible.cfg:
```
private_key_file = ~/.ssh/express42
```
Change IP address of freeradius host in ```hosts``` file.


Look into defaults and change ```asa_internal_iface_ip``` to the Cisco ASA's **inside** interface.

Also, please note the value of ```shared_secret``` variable, as it will be used later in the Cisco ASA config.

### How to run?

You can use the following command:
```
ansible-playbook playbooks/freeradius.yml
```
