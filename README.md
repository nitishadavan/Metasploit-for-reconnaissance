# Metasploit-for-reconnaissance
# Metasploit
Metasploit for reconnaissance in pentesting

# AIM:

To get introduced to Metasploit Framework and to  perform reconnaissance  in pentesting .

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

## EXECUTION STEPS AND ITS OUTPUT:
Find out the ip address of the attackers system
## OUTPUT:

![image](https://github.com/user-attachments/assets/285a295b-2efa-48e6-96c7-7a550a78083b)

Invoke msfconsole:
## OUTPUT:


![image](https://github.com/user-attachments/assets/a36d6a72-c0ae-47c1-9ea2-4dd2a9c24f71)

Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.

## OUTPUT:
![Screenshot 2025-04-21 183926](https://github.com/user-attachments/assets/1d1d5428-dfae-4988-8d51-ae4926da9e5d)

![image](https://github.com/user-attachments/assets/4a4bceb0-5200-49aa-82c8-cef5128c275b)

![image](https://github.com/user-attachments/assets/9a6f91ae-90f1-4a2e-a679-ad3edae39159)

![image](https://github.com/user-attachments/assets/773b731c-03a5-49f9-84ba-2b5f1372796e)

![image](https://github.com/user-attachments/assets/7b3032ef-5642-415a-ba67-30b8776c85b6)

Following command is executed for scanning the systems on our local area network with a TCP scan (-sT) looking for open ports between 1 and 1000 (-p1-1000).
msf >  nmap -sT 192.168.228.34/24 -p1-1000
## OUTPUT:

![image](https://github.com/user-attachments/assets/6a36de9b-c0a7-475f-b6bd-9d601df0fb57)

use the db-nmap command to scan and save the results into Metasploit's postgresql attached database. In that way, you can use those results in the exploitation stage later.

scan the targets with the command db_nmap as follows.
msf > db_nmap 192.168.228.34/24
## OUTPUT:

![image](https://github.com/user-attachments/assets/5dfe879f-03cb-4e89-b8d4-108cd9227f49)

![image](https://github.com/user-attachments/assets/a38eac13-5de3-4ed4-8905-57de555ac089)

Metasploit has a multitude of scanning modules built in. If we open another terminal, we can navigate to Metasploit's auxiliary modules and list all the scanner modules.
cd /usr/share /metasploit-framework/modules/auxiliary
kali > ls -l
## OUTPUT:

![image](https://github.com/user-attachments/assets/b789454c-d07c-4e33-a1b3-43773fef3fca)

Search is a powerful command in Metasploit that you can use to find what you want to locate. 
msf >search name:Microsoft type:exploit
## OUTPUT:
![image](https://github.com/user-attachments/assets/27f039fe-2060-4831-a75e-72e6ee247019)


The info command provides information regarding a module or platform,
## OUTPUT:
![image](https://github.com/user-attachments/assets/efbf406d-bd26-4e99-b2d0-65f005b93d4c)

##MYSQL ENUMERATION
Find the IP address of the Metasploitable machine first. Then, use the db_nmap command in msfconsole with Nmap flags to scan the MySQL database at 3306 port.
db_nmap -sV -sC -p 3306 <metasploitable_ip_address>
## OUTPUT:
![image](https://github.com/user-attachments/assets/f7867d89-fb6f-4453-9d3f-5c4c48990a48)


![image](https://github.com/user-attachments/assets/bfc9b8a1-5585-4dab-b7af-6c5332b7f7be)

![image](https://github.com/user-attachments/assets/16a40d31-2af7-441a-a4f5-dcd31f74b11b)

![image](https://github.com/user-attachments/assets/9bee1c00-b270-4e47-9fca-d7a4382800a8)

## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
