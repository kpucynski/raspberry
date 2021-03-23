Raspberry Pi provision
======================

Quickly make new Raspberry Pi with fresh Raspbian usable.

```bash
sudo apt install sshpass
ansible-playbook -i hosts provision.yml --extra-vars target_hostname=some-name
```
