# workshop-demo

Small demo playbooks for network automation.

Install Python requirements (especially for NX-OS automation):

```console
pip3 install -r requirements.txt
```

Install Ansible requirements:

```console
ansible-galaxy collection install -r collections/requirements.yml
```

## NX-OS demo

After installing the requirements, fill the necessary connection details in `group_vars/nxos.yml`.

Run the playbook:

```console
ansible-playbook -i inventory.ini nxos_demo.yml
```

## ACI demo

After installing the requirements, export the necessary environment variables, e.g.

```console
export ACI_HOST=sandboxapicdc.cisco.com
```

Run the playbook:

```console
ansible-playbook aci_demo.yml
```
