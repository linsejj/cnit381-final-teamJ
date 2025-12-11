# cnit381-final-teamJ
Names: Josh Linse & Johnathon Laun

Project Description: This project focused on us creating ansible playbooks to automate the configurations for 2 routers and a switch. This includes creating VLANS, loopback interfaces, EIGRP configurations, backing up configurations, verifying connectivity, and testing the results. We also created a network topology diagram.

How to Run playbooks:

ansible-playbook -i /location/of/inventory.ini /location/of/playbook.yaml

Playbooks:
01_verify_connectivity.yaml    - shows version of each device

02_base_config.yaml            - adds descriptions & hostnames on each device

03_eigrp_config.yaml           - configures EIGRP and loopbacks on each router

04_vlan_config.yaml            - creates VLANs on switch & subinterfaces on routers

05_services_config.yaml        - Adds NTP to devices & enables logging

06_backup_config.yaml          - Backups each configuration to host device
