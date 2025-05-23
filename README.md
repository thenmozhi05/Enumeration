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

##  Output

![316322654-672e48cd-bdff-40d3-bea6-e71a504bb773](https://github.com/pradeepasri26/Enumeration/assets/131433142/25b266d8-59b6-450c-b6a2-a1d57a2e24ef)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

## Output

![316322697-51cd5a33-0e76-45b8-bd77-3e25cb0c85d9](https://github.com/pradeepasri26/Enumeration/assets/131433142/bea236ad-764b-49ed-8f58-b85a3e435603)

intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

## Output

![316322730-aef55b0e-18e2-4974-aafa-1ecf9eaa3f21](https://github.com/pradeepasri26/Enumeration/assets/131433142/7dc29339-8ec1-4f2a-a263-81e11a498f55)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

## Output

![316322768-31fe3a2c-b3da-4d35-9af2-c5664f0fe7d0](https://github.com/pradeepasri26/Enumeration/assets/131433142/4d74b3b4-9097-45a8-a400-e88f877d3655)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

## Output

![316322834-79c49be8-66ba-498e-bf2f-cae562650f07](https://github.com/pradeepasri26/Enumeration/assets/131433142/5aac3010-e3da-47bf-ad0b-9291c7e476fa)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

## Output

![316322861-29c2b50d-285f-4eb9-8db9-7739afcecc4b](https://github.com/pradeepasri26/Enumeration/assets/131433142/d2a33d93-4821-497e-9f7b-f7e9ef513de0)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

## Output

![316322876-c044539d-c4c3-4667-a2bd-2718d810e7fc](https://github.com/pradeepasri26/Enumeration/assets/131433142/cdc33fc0-3ab2-4440-afbb-f0081c016c3d)

#DNS Enumeration 
##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
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

##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same

#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

