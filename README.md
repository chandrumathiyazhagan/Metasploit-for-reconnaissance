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

![image](https://github.com/chandrumathiyazhagan/Metasploit-for-reconnaissance/assets/119393023/2ad3515c-5fd0-4459-8861-e967cd9d7158)

Invoke msfconsole

![WhatsApp Image 2024-04-28 at 11 38 36_53dc1558](https://github.com/chandrumathiyazhagan/Metasploit-for-reconnaissance/assets/119393023/95d0ae46-57da-4b87-9c5b-3ef0b4a7f3c2)

Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.

![image](https://github.com/chandrumathiyazhagan/Metasploit-for-reconnaissance/assets/119393023/717b5daa-6c3b-42eb-a821-ac379c96e98f)

### Port scanning:
msf > nmap -sT 192.168.1810/24-p1-1000

![image](https://github.com/chandrumathiyazhagan/Metasploit-for-reconnaissance/assets/119393023/0f9285c1-0aad-416b-8538-b107458ff514)

msf > db_nmap 192.168.181.0/24

![image](https://github.com/chandrumathiyazhagan/Metasploit-for-reconnaissance/assets/119393023/e09ca19a-5338-490b-855f-53fac79dbca2)

kali > ls-l

![image](https://github.com/chandrumathiyazhagan/Metasploit-for-reconnaissance/assets/119393023/25a1060e-c0cb-47f1-b231-b0a82effe102)

search

![image](https://github.com/chandrumathiyazhagan/Metasploit-for-reconnaissance/assets/119393023/de158985-d6cd-471c-a65f-083ca313acb7)

info

![image](https://github.com/chandrumathiyazhagan/Metasploit-for-reconnaissance/assets/119393023/3ae84d77-dc71-463b-8863-4d5bd2d74563)

### MYSQL ENUMERATION
db_nmap -sV -sC -p 3306 <metasploitable_ip_address>

![image](https://github.com/chandrumathiyazhagan/Metasploit-for-reconnaissance/assets/119393023/600cec99-6b47-4426-a283-719fba11c7a0)

search

![image](https://github.com/chandrumathiyazhagan/Metasploit-for-reconnaissance/assets/119393023/8ef27781-c056-43a4-ba4e-e3355d1eed8c)

use 11 Or: use auxiliary/scanner/mysql/mysql_version

![image](https://github.com/chandrumathiyazhagan/Metasploit-for-reconnaissance/assets/119393023/68e42eaa-11f7-45b7-bc8c-a86d0ce8ce85)

Use the set rhosts command to set the parameter and run the module, as follows:

![image](https://github.com/chandrumathiyazhagan/Metasploit-for-reconnaissance/assets/119393023/67eabc55-3079-4efc-8c47-1772d4d7c684)

After scanning, you can also brute force MySQL root account via Metasploit's auxiliary(scanner/mysql/mysql_login) module

![image](https://github.com/chandrumathiyazhagan/Metasploit-for-reconnaissance/assets/119393023/6faf7ee8-2e8a-4c47-a4cd-7c839b838e2e)

/usr/share/wordlists: set PASS_FILE /usr/share/wordlistss/rockyou.txt

![image](https://github.com/chandrumathiyazhagan/Metasploit-for-reconnaissance/assets/119393023/a56ed6b8-9913-45c2-9ad7-9894eeb0c237)

![image](https://github.com/chandrumathiyazhagan/Metasploit-for-reconnaissance/assets/119393023/4894cf65-54b1-4fd5-ac4f-a63dc0b518ef)

## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
