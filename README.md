# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com

![e3 1](https://github.com/Gayathriraj18/Enumeration/assets/94154854/bb8ccb3f-3d37-48ff-affd-8addf4d14878)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

![e3 2](https://github.com/Gayathriraj18/Enumeration/assets/94154854/90205c84-8d3c-4e30-9b58-db0d4e69ff41)



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![e3 3](https://github.com/Gayathriraj18/Enumeration/assets/94154854/d71f8702-4f4d-45a4-a3d8-1fe5c11bbe7d)



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

![e3 4](https://github.com/Gayathriraj18/Enumeration/assets/94154854/33ffbf8f-760f-4e1c-8765-b00aa9019e9e)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![e3 5](https://github.com/Gayathriraj18/Enumeration/assets/94154854/192a9f3a-7002-48d4-ad65-c86f1bbddac2)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![e3 6](https://github.com/Gayathriraj18/Enumeration/assets/94154854/71ea607a-55f3-4810-b40d-1023b9752a53)


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![e3 7](https://github.com/Gayathriraj18/Enumeration/assets/94154854/c0ab793a-2501-4870-8aab-02e36fb3d77f)

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:

Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion

## OUTPUT:

![e3 8](https://github.com/Gayathriraj18/Enumeration/assets/94154854/688ff8aa-be4c-4b64-b45a-1c41673d6370)

![e3 9](https://github.com/Gayathriraj18/Enumeration/assets/94154854/eb7b7627-e987-4c73-beac-7900590a33ed)





##dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.


![e3 10](https://github.com/Gayathriraj18/Enumeration/assets/94154854/a01de89d-d556-4d66-a1f7-c2ffd4ec6c60)


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

![e3 11](https://github.com/Gayathriraj18/Enumeration/assets/94154854/2004dce6-f6d9-4891-bdf2-31130a977763)



In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

![e3 12](https://github.com/Gayathriraj18/Enumeration/assets/94154854/e84c9d1c-4240-4f27-8228-5dfe8bc65697)


select any username in the first column of the above file and check the same

![e3 13](https://github.com/Gayathriraj18/Enumeration/assets/94154854/f23e1738-e83f-4641-b47a-0800fe323c57)


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands

![e3 14](https://github.com/Gayathriraj18/Enumeration/assets/94154854/51bc5b66-a152-413d-95d3-eba53a2dac93)

  

  
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

![e3 15](https://github.com/Gayathriraj18/Enumeration/assets/94154854/743dfff6-2d13-446d-817e-f889f9b20f58)



## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully.

