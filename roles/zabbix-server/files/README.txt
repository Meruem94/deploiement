# file: /roles/zabbix/files/README.txt

# Zabbix_server
Username=Admin
Password=zabbix
Note : After first connexion change user Password
  - Profile -> User

# Zabbix_server informations
Zabbix server v2.2.20 (revision 72882) (25 September 2017)
Compilation time: Sep 26 2017 23:21:26

# Databases
database_name=zabbix
database_password=zabbix

# Below all commands to delete all iptables rules
iptables -F
iptables -X
iptables -t nat -F
iptables -t nat -X
iptables -t mangle -F
iptables -t mangle -X
iptables -P INPUT ACCEPT
iptables -P FORWARD ACCEPT
iptables -P OUTPUT ACCEPT
