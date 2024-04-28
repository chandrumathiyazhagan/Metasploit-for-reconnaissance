# Metasploit-for-reconnaissance
Metasploit for reconnaissance in pentesting

# AIM:

To get introduced to Metasploit Framework and to  perform reconnaissance  in pentesting .

## DESIGN STEPS:

- `Step 1:` Install kali linux either in partition or virtual box or in live mode

- `Step 2:` Investigate on the various categories of tools as follows:

- `Step 3:` Open terminal and try execute some kali linux commands

## EXECUTION STEPS AND ITS OUTPUT:
Find out the ip address of the attackers system

![5 1](https://github.com/SaiPraneeth04/Metasploit-for-reconnaissance/assets/119390353/c514f8b3-996f-4e06-8898-f37a346b28ad)


Invoke msfconsole

![5 2](https://github.com/SaiPraneeth04/Metasploit-for-reconnaissance/assets/119390353/167fdf48-8a0d-47c4-9d3a-b6d6183068dd)


Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.

![5 3](https://github.com/SaiPraneeth04/Metasploit-for-reconnaissance/assets/119390353/e970d313-a297-4521-9967-3a09c698504e)


### Port scanning:
msf > nmap -sT 192.168.1810/24-p1-1000

![5 4](https://github.com/SaiPraneeth04/Metasploit-for-reconnaissance/assets/119390353/b7faa450-2a59-4005-a518-c62cd2112ca3)


msf > db_nmap 192.168.181.0/24

![5 5](https://github.com/SaiPraneeth04/Metasploit-for-reconnaissance/assets/119390353/19ec99f4-905e-4667-8cef-4550fb17f9d8)


kali > ls-l

![5 6](https://github.com/SaiPraneeth04/Metasploit-for-reconnaissance/assets/119390353/983c051d-84f1-45e5-938d-c04d8b1cd3d4)


search

![5 7](https://github.com/SaiPraneeth04/Metasploit-for-reconnaissance/assets/119390353/c6aebc51-73fa-4f7d-b1f7-0f76e1241497)



info

![5 8](https://github.com/SaiPraneeth04/Metasploit-for-reconnaissance/assets/119390353/3906c41b-e9cf-4260-9776-429252a84e93)



### MYSQL ENUMERATION
db_nmap -sV -sC -p 3306 <metasploitable_ip_address>

![5 9](https://github.com/SaiPraneeth04/Metasploit-for-reconnaissance/assets/119390353/92a1e398-3df3-4652-bb6f-65238378ec94)


search

![5 10](https://github.com/SaiPraneeth04/Metasploit-for-reconnaissance/assets/119390353/72989cd9-3330-4808-bd62-12752eda7071)


use 11 Or: use auxiliary/scanner/mysql/mysql_version


![5 11](https://github.com/SaiPraneeth04/Metasploit-for-reconnaissance/assets/119390353/c4c5ed30-2a0b-4786-a3e6-b533cf67407d)


Use the set rhosts command to set the parameter and run the module, as follows:

![5 12](https://github.com/SaiPraneeth04/Metasploit-for-reconnaissance/assets/119390353/80102490-7c73-43f9-99f4-a75969d15dff)



After scanning, you can also brute force MySQL root account via Metasploit's auxiliary(scanner/mysql/mysql_login) module

![5 13](https://github.com/SaiPraneeth04/Metasploit-for-reconnaissance/assets/119390353/d4e9204f-7784-4af3-8e96-663f9e84b44f)



/usr/share/wordlists: set PASS_FILE /usr/share/wordlistss/rockyou.txt

![5 14](https://github.com/SaiPraneeth04/Metasploit-for-reconnaissance/assets/119390353/32cce3bd-c699-48c5-8f8a-74a69242ec94)


![5 15](https://github.com/SaiPraneeth04/Metasploit-for-reconnaissance/assets/119390353/8a0efc14-40b4-416f-a11e-f5a52c4996a9)



## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
