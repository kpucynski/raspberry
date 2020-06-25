Home-Assistant on RPI
=====================

Tools for provisioning home-assistant on RPI

```bash
ansible-playbook -v -i hosts --vault-password-file .vault_pass some-assistant.yml --extra-vars iscsi_create_fs=false
ansible-playbook -v -i hosts --vault-password-file .vault_pass home-assistant.yml --tags ha
ansible-playbook -v -i hosts --vault-password-file .vault_pass home-assistant.yml --tags config
```

# Notes

I'm using two separate RTL SDR receivers for fr24feed (Flightradar24 data sharing)
and rtl433 (weather station data). Unfortunately it is impossible to distinguish them:
enumerating order is not reliable and serial number on both cards is '1'.
The only way is to verify that dump1090 (for fr24feed) is using different device
index than rtl_433.
