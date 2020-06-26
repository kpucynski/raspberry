FlightRadar24
=============

Quick installation of FlighRadar24 ADS-B data sharing tool.

Take Sharing Key from https://www.flightradar24.com/account/data-sharing and run:

```bash
ansible-playbook -v -i hosts fr24.yml --extra-vars fr24_key=FR24_SHARING_KEY
```


