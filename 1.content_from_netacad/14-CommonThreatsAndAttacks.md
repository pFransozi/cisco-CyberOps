# 14 Common Threats and Attacks

## Malware

### Types of malware

Malware is short for malicious software or malicious code. It is code or software that is specifically designed to damage, disrupt, steal, or generally inflict some other “bad” or illegitimate action on data, hosts, or networks. It is important to know about malware because threat actors and online criminals frequently try to trick users into installing malware to help exploit security gaps.

#### Viruses

A virus is a type of malware that **spreads by inserting a copy of itself into another program**. After the program is run, viruses then spread from one computer to another, infecting the computers. **Most viruses require human help to spread**. Viruses can lay dormant for an extended period and then activate at a specific time and date.

A simple virus may install itself at the first line of code in an executable file. When activated, the virus might check the disk for other executables so that it can infect all the files it has not yet infected. Viruses can be harmless, such as those that display a picture on the screen, or they can be destructive, such as those that modify or delete files on the hard drive. Viruses can also be programmed to mutate to avoid detection.

Most viruses are now spread by USB memory drives, CDs, DVDs, network shares, and email. Email viruses are a common type of virus.

#### Trojan Horses

Trojan horse malware is software that appears to be legitimate, but it contains malicious code which exploits the privileges of the user that runs it. Often, Trojans are found attached to online games. Users are commonly tricked into loading and executing the Trojan horse on their systems. While playing the game, the user will not notice a problem. In the background, the Trojan horse has been installed on the user’s system. The malicious code from the Trojan horse continues operating even after the game has been closed. The Trojan horse concept is flexible. It can cause immediate damage, provide remote access to the system, or access through a back door. It can also perform actions as instructed remotely, such as "send me the password file once per week." This tendency of malware to send data back to the cybercriminal highlights the need to monitor outbound traffic for attack indicators.

Custom-written Trojan horses, such as those with a specific target, are difficult to detect.

##### Trojan Horse Classification

Trojan horses are usually classified according to the damage that they cause, or the manner in which they breach a system.

|Type of Trojan Horse|Description|
|--------------------|-----------|
|Remote-access|Enables unauthorized remote access|
|Data-sending|Provides the threat actor with sensitive data, such as passwords|
|Destructive|Corrupts or deletes files|
|Proxy|Uses the victim's computer as the source device to launch attacks and perform other illegal activities|
|FTP|Enables unauthorized file transfer services on end devices|
|Security software disabler|Stops antivirus programs or firewalls from functioning|
|Denial of Service (DoS)|Slows or halts network activity|
|Keylogger|Actively attempts to steal confidential information, such as credit card numbers, by recording keystrokes entered into a web form|

#### Worms

Computer worms are similar to viruses because they replicate and can cause the same type of damage. Specifically, worms replicate themselves by independently exploiting vulnerabilities in networks. Worms can slow down networks as they spread from system to system. Whereas a virus requires a host program to run, worms can run by themselves. Other than the initial infection, they no longer require user participation. After a host is infected, the worm is able to spread very quickly over the network.

Worms are responsible for some of the most devastating attacks on the internet. In 2001, the Code Red worm had initially infected 658 servers. Within 19 hours, the worm had infected over 300,000 servers.

The initial infection of the SQL Slammer worm is known as the worm that ate the internet. SQL Slammer was a denial of service (DoS) attack that exploited a buffer overflow bug in Microsoft’s SQL Server. At its peak, the number of infected servers doubled in size every 8.5 seconds. This is why it was able to infect 250,000+ hosts within 30 minutes. When it was released on the weekend of January 25, 2003, it disrupted the internet, financial institutions, ATM cash machines, and more. Ironically, a patch for this vulnerability had been released 6 months earlier. The infected servers did not have the updated patch applied. This was a wake-up call for many organizations to implement a security policy requiring that updates and patches be applied in a timely fashion.

Worms share similar characteristics. They all exploit an enabling vulnerability, have a way to propagate themselves, and they all contain a payload.

##### Worm Components

Most worm attacks consist of three components, as listed in the animation above.

* **Enabling vulnerability**: A worm installs itself using an exploit mechanism, such as an email attachment, an executable file, or a Trojan horse, on a vulnerable system.
* **Propagation mechanism**: After gaining access to a device, the worm replicates itself and locates new targets.
* **Payload**: Any malicious code that results in some action is a payload. Most often this is used to create a backdoor that allows a threat actor access to the infected host or to create a DoS attack.

#### Ransomware

Threat actors have used viruses, worms, and Trojan horses to carry their payloads and for other malicious reasons. However, malware continues to evolve.

Currently, the most dominating malware is ransomware. Ransomware is malware that denies access to the infected computer system or its data. The cybercriminals then demand payment to release the computer system.

Ransomware has evolved to become the most profitable malware type in history. In the first half of 2016, ransomware campaigns targeting both individual and enterprise users became more widespread and potent.

There are dozens of ransomware variants. Ransomware frequently uses an encryption algorithm to encrypt system files and data. The majority of known ransomware encryption algorithms cannot be easily decrypted, leaving victims with little option but to pay the asking price. Payments are typically paid in Bitcoin because users of bitcoin can remain anonymous. Bitcoin is an open-source, digital currency that nobody owns or controls.

Email and malicious advertising, also known as malvertising, are vectors for ransomware campaigns. Social engineering is also used, as when cybercriminals who identify themselves as security technicians call homes and persuade users to connect to a website that downloads the ransomware to the user’s computer..

#### Other Malware

|Type of Malware|Description|
|---------------|-----------|
|Spyware|Used to gather information about a user and send the information to another entity without the user’s consent. Spyware can be a system monitor, Trojan horse, Adware, tracking cookies, and key loggers|
|Adware|Displays annoying pop-ups to generate revenue for its author. The malware may analyze user interests by tracking the websites visited. It can then send pop-up advertising pertinent to those sites|
|Scareware|Includes scam software which uses social engineering to shock or induce anxiety by creating the perception of a threat. It is generally directed at an unsuspecting user and attempts to persuade the user to infect a computer by taking action to address the bogus threat|
|Phishing|Attempts to convince people to divulge sensitive information. Examples include receiving an email from their bank asking users to divulge their account and PIN numbers|
|Rootkits|Installed on a compromised system. After it is installed, it continues to hide its intrusion and provide privileged access to the threat actor|

#### Common Malware Behaviors

Cybercriminals continually modify malware code to change how it spreads and infects computers. However, most produce similar symptoms that can be detected through network and device log monitoring. Computers infected with malware often exhibit one or more of the following symptoms:

* Appearance of strange files, programs, or desktop icons
* Antivirus and firewall programs are turning off or reconfiguring settings
* Computer screen is freezing or system is crashing
* Emails are spontaneously being sent without your knowledge to your contact list
* Files have been modified or deleted
* Increased CPU and/or memory usage
* Problems connecting to networks
* Slow computer or web browser speeds
* Unknown processes or services running
* Unknown TCP or UDP ports open
* Connections are made to hosts on the Internet without user action
* Strange computer behavior

### Check Your Understanding - Malware

1. What type of malware executes arbitrary code and installs copies of itself in the memory of the infected computer? The main purpose of this malware is to automatically replicate from system to system across the network. **worm**
2. What type of malware typically displays annoying pop-ups to generate revenue for its author?   **adware**
3. What type of malware encrypts all data on a drive and demands payment in Bitcoin cryptocurrence to unencrypt the files? **ransomware**
4. What type of malware attempts to convince people to divulge their personally identifable information (PII)? phishing

## Common Network Attacks - Reconnaissance, Access, and Social Engineering

### Types of Network Attacks

Malware is a means to get a payload delivered. When it is delivered and installed, the payload can be used to cause a variety of network-related attacks from the inside. Threat actors can also attack the network from outside.

Why do threat actors attack networks? There are many motives including money, greed, revenge, or political, religious, or sociological beliefs. Network security professionals must understand the types of attacks used to counter these threats to ensure the security of the LAN.

To mitigate attacks, it is useful to first categorize the various types of attacks. By categorizing network attacks, it is possible to address types of attacks rather than individual attacks.

Although, there is no standardized way of categorizing network attacks, the method used in this course classifies attacks in three major categories.

* Reconnaissance Attacks
* Access Attacks
* DoS Attacks

#### Reconnaissance Attacks

Reconnaissance is information gathering. Threat actors use reconnaissance (or recon) attacks to do unauthorized discovery and mapping of systems, services, or vulnerabilities. Recon attacks precede access attacks or DoS attacks.

|Technique|Description|
|---------|-----------|
| Perform an information query of a target |  The threat actor is looking for initial information about a target. Various tools can be used, including the Google search, organizations website, whois, and more|
| Initiate a ping sweep of the target network | The information query usually reveals the target’s network address. The threat actor can now initiate a ping sweep to determine which IP addresses are active|
| Initiate a port scan of active IP addresses | This is used to determine which ports or services are available. Examples of port scanners include Nmap, SuperScan, Angry IP Scanner, and NetScanTools|
| Run vulnerability scanners | This is to query the identified ports to determine the type and version of the application and operating system that is running on the host. Examples of tools include Nipper, Secuna PSI, Core Impact, Nessus v6, SAINT, and Open VAS|
| Run exploitation tools | The threat actor now attempts to discover vulnerable services that can be exploited. A variety of vulnerability exploitation tools exist including Metasploit, Core Impact, Sqlmap, Social Engineer Toolkit, and Netsparker|

### Access Attacks

Access attacks exploit known vulnerabilities in authentication services, FTP services, and web services. The purpose of this type of attack is to gain entry to web accounts, confidential databases, and other sensitive information. Threat actors use access attacks on network devices and computers to retrieve data, gain access, or to escalate access privileges to administrator status. 

#### Password Attacks

In a password attack, the threat actor attempts to discover critical system passwords using various methods. Password attacks are very common and can be launched using a variety of password cracking tools.

#### Spoofing Attacks

In spoofing attacks, the threat actor device attempts to pose as another device by falsifying data. Common spoofing attacks include IP spoofing, MAC spoofing, and DHCP spoofing.

Other Access attacks include:

* Trust exploitations
* Port redirections
* Man-in-the-middle attacks
* Buffer overflow attacks

### Social Engineering Attacks

Social engineering is an access attack that attempts to manipulate individuals into performing actions or divulging confidential information. Some social engineering techniques are performed in-person while others may use the telephone or internet.

Social engineers often rely on people’s willingness to be helpful. They also prey on people’s weaknesses. For example, a threat actor could call an authorized employee with an urgent problem that requires immediate network access. The threat actor could appeal to the employee’s vanity, invoke authority using name-dropping techniques, or appeal to the employee’s greed.

|Social Engineering Attack|Description|
|-------------------------|-----------|
|Pretexting|A threat actor pretends to need personal or financial data to confirm the identity of the recipient|
|Phishing| A threat actor sends fraudulent email which is disguised as being from a legitimate, trusted source to trick the recipient into installing malware on their device, or to share personal or financial information|
|Spear phishing| A threat actor creates a targeted phishing attack tailored for a specific individual or organization|
|Spam| Also known as junk mail, this is unsolicited email which often contains harmful links, malware, or deceptive content|
|Something for Something| Sometimes called “Quid pro quo”, this is when a threat actor requests personal information from a party in exchange for something such as a gift|
|Baiting| A threat actor leaves a malware infected flash drive in a public location. A victim finds the drive and unsuspectingly inserts it into their laptop, unintentionally installing malware|
|Impersonation| In this type of attack, a threat actor pretends to be someone else to gain the trust of a victim|
|Tailgating| This is where a threat actor quickly follows an authorized person into a secure location to gain access to a secure area|
|Shoulder surfing| This is where a threat actor inconspicuously looks over someone’s shoulder to steal their passwords or other information|
|Dumpster diving| This is where a threat actor rummages through trash bins to discover confidential documents|

The Social Engineer Toolkit (SET) was designed to help white hat hackers and other network security professionals create social engineering attacks to test their own networks. It is a set of menu-based tools that help launch social engineering attacks. The SET is for educational purposes only. It is freely available on the internet. Enterprises must educate their users about the risks of social engineering, and develop strategies to validate identities over the phone, via email, or in person.

* Protecting against social engineering attacks
  * never leave your username/password credentials where they can easily be found
  * never open emails from untrusted source
  * never release work related information on social media sites
  * never re-use work related passwords
  * always lock or sign out of your computer when unattended
  * always report suspicious individuals
  * always destroy confidential information according to the organization policy.

### Strengthening the Weakest Link

Cybersecurity is only as strong as its weakest link. Since computers and other internet-connected devices have become an essential part of our lives, they no longer seem new or different. People have become very casual in their use of these devices and rarely think about network security. The weakest link in cybersecurity can be the personnel within an organization, and social engineering a major security threat. Because of this, one of the most effective security measures that an organization can take is to train its personnel and create a “security-aware culture.”

### Denial of Service, Buffer Overflows, and Evasion

A Denial of Service (DoS) attack **creates some sort of interruption of network services** to users, devices, or applications. There are two major types of DoS attacks:

* **Overwhelming Quantity of Traffic**: The threat actor sends an enormous quantity of data at a rate that the network, host, or application cannot handle. This causes transmission and response times to slow down. It can also crash a device or service.
* **Maliciously Formatted Packets**: The threat actor sends a maliciously formatted packet to a host or application and the receiver is unable to handle it. This causes the receiving device to run very slowly or crash.

* **DoS**: DoS attacks are a major risk because they interrupt communication and cause significant loss of time and money. These attacks are relatively simple to conduct, even by an unskilled threat actor.
* **DDoS**: A Distributed DoS Attack (DDoS) is similar to a DoS attack, but it originates from multiple, coordinated sources. For example, A threat actor builds a network of infected hosts, known as zombies. The threat actor uses a command and control (CnC) system to send control messages to the zombies. The zombies constantly scan and infect more hosts with bot malware. The bot malware is designed to infect a host, making it a zombie that can communicate with the CnC system. The collection of zombies is called a botnet. When ready, the threat actor instructs the CnC system to make the botnet of zombies carry out a DDoS attack.

#### Components of DDoS Attacks

A DDoS attack can use hundreds or thousands of sources, **as in IoT-based DDoS attacks**.

|Component|Description|
|---------|-----------|
|zombies|This refers to a group of compromised hosts (i.e., agents). These hosts run malicious code referred to as robots (i.e., bots). The zombie malware continually attempts to self-propagate like a worm|
|bots|Bots are malware that is designed to infect a host and communicate with a handler system. Bots can also log keystrokes, gather passwords, capture and analyze packets, and more|
|botnet|This refers to a group of zombies that have been infected using self-propagating malware (i.e., bots) and are controlled by handlers|
|handlers|This refers to a primary command-and-control (CnC or C2) server controlling groups of zombies. The originator of a botnet can use Internet Relay Chat (IRC) or a web server on the C2 server to remotely control the zombies|
|botmaster|This is the threat actor who is in control of the botnet and handlers|

**Note: There is an underground economy where botnets can be bought (and sold) for a nominal fee. This can provide threat actors with botnets of infected hosts ready to launch a DDoS attack against the target of choice.**

#### Mirai Botnet

Mirai is malware that targeted IoT devices that are configured with default login information. Closed-circuit television (CCTV) cameras made up the majority of Mirai’s targets. Using a brute force dictionary attack, Mirai ran through a list of default usernames and passwords that were widely known on the internet.

After gaining successful access, Mirai targeted the Linux-based BusyBox utilities that run on these devices. These utilities were used to turn the devices into bots that could be remotely controlled as part of a botnet. The botnet was then used as part of a distributed denial of service (DDoS) attack. In September 2016, a Mirai botnet of over 152,000 CCTVs and digital video recorders (DVRs) was responsible for the largest DDoS attack known until that time. With peak traffic of over 1 Tb/s, it took down the hosting services of a France-based web hosting company.

In October 2016 the services of Dyn, a domain name service (DNS) provider, were attacked, causing internet outages for millions of users in the United States and Europe.

### Buffer Overflow

The goal of a threat actor when using a buffer overflow DoS attack is **to find a system memory-related flaw on a server and exploit it**. Exploiting the buffer memory by overwhelming it with unexpected values usually renders the system inoperable, creating a DoS attack.

An early example of using malformed packets was the Ping of Death. In this legacy attack, the threat actor sent a ping of death, which was an echo request in an IP packet larger than the maximum packet size of 65,535 bytes. The receiving host would not be able to handle a packet of that size and it would crash. **Buffer overflow attacks are continually evolving**. For instance, a remote denial of service attack vulnerability was recently discovered in Microsoft Windows 10. Specifically, a threat actor created malicious code to access out-of-scope memory. When this code is accessed by the Windows AHCACHE.SYS process, it attempts to trigger a system crash, denying service to the user. Search the Internet on “TALOS-2016-0191 blog” to go to the Cisco Talos threat intelligence website and read a description of such an attack.

**Note: It is estimated that one third of malicious attacks are the result of buffer overflows.**

### Evasion Methods

Threat actors learned long ago that “to hide is to thrive”. This means their malware and attack methods are most effective when they are undetected. For this reason, many attacks use stealthy evasion techniques to disguise an attack payload. Their goal is to prevent detection by evading network and host defenses.

|Evasion Method|Description|
|--------------|-----------|
|Encryption and tunneling|This evasion technique uses tunneling to hide, or encryption to scramble, malware files. This makes it difficult for many security detection techniques to detect and identify the malware. Tunneling can mean hiding stolen data inside of legitimate packets|
|Resource exhaustion|This evasion technique makes the target host too busy to properly use security detection techniques|
|Traffic fragmentation|This evasion technique splits a malicious payload into smaller packets to bypass network security detection. After the fragmented packets bypass the security detection system, the malware is reassembled and may begin sending sensitive data out of the network|
|Protocol-level misinterpretation|This evasion technique occurs when network defenses do not properly handle features of a PDU like a checksum or TTL value. This can trick a firewall into ignoring packets that it should check|
|Traffic substitution|In this evasion technique, the threat actor attempts to trick an IPS by obfuscating the data in the payload. This is done by encoding it in a different format. For example, the threat actor could use encoded traffic in Unicode instead of ASCII. The IPS does not recognize the true meaning of the data, but the target end system can read the data|
|Traffic insertion|Similar to traffic substitution, but the threat actor inserts extra bytes of data in a malicious sequence of data. The IPS rules miss the malicious data, accepting the full sequence of data|
|Pivoting|This technique assumes the threat actor has compromised an inside host and wants to expand their access further into the compromised network. An example is a threat actor who has gained access to the administrator password on a compromised host and is attempting to login to another host using the same credentials|
|Rootkits|A rootkit is a complex attacker tool used by experienced threat actors. It integrates with the lowest levels of the operating system. When a program attempts to list files, processes, or network connections, the rootkit presents a sanitized version of the output, eliminating any incriminating output. The goal of the rootkit is to completely hide the activities of the attacker on the local system|
|Proxies|Network traffic can be redirected through intermediate systems in order to hide the ultimate destination for stolen data. In this way, known command-and-control not be blocked by an enterprise because the proxy destination appears benign. Additionally, if data is being stolen, the destination for the stolen data can be distributed among many proxies, thus not drawing attention to the fact that a single unknown destination is serving as the destination for large amounts of network traffic|

## Check Your Understanding - Identify the Types of Network Attacks

1. What is the weakest link in network security? **ACCESS**
   Man-in-the-Middle is an access attack in which the threat actor is positioned between legitimate entities in order to read or modify the data that passes between them.

2. What type of attack is tailgating? **SOCIAL ENGINEERING**
   Tailgating is a social engineering attack where a threat actor quickly follows an authorized person into a secure location by taking advantage of the authorized person’s credentials.

3. What type of attack is port scanning? **RECONNAISSANCE**
   Port scanning is a reconnaissance attack in which a threat actor uses a tool like Nmap to scan for open TCP or UDP ports on active devices in a network.

4. What is the weakest link in network security? **PEOPLE**
   In any organization, people can be weakest link in network security. People fall victim to social engineering attacks, open file attachments that contain malware, or use insecure passwords, for example.


## Common Threats and Attacks Summary

* **Malware**: Malware is short for malicious software or malicious code. Threat actors frequently try to trick users into installing malware to help exploit end device vulnerabilities. Often antimalware software cannot be updated quickly enough to stop new threats. Three common types are virus, worm, and Trojan horse. A virus is a type of malware that spreads by inserting a copy of itself into another program. Most viruses are spread through USB memory drives, CDs, DVDs, network shares, and email. Trojan horse malware is software that appears to be legitimate, but it contains malicious code that exploits the privileges of the user that runs it. Often, Trojans are found on online games. Trojan horses are usually classified according to the damage they cause. Types of Trojan horses include remote-access, data-sending, destructive, proxy, FTP, security software disabler, DoS, and keylogger. Worms are similar to viruses because they replicate and can cause the same type of damage. Viruses require a host program to run. Worms can run themselves. Most worm attacks consist of three components: enabling vulnerability, propagation mechanism, and payload. Currently, ransomware is the most dominant malware. It denies access to the infected system or its data. The cybercriminals then demand payment to release the computer system. Other malware examples include spyware, adware, scareware, phishing, and rootkits.

* **Common Network Attacks – Reconnaissance, Access, and Social Engineering**: Threat actors can also attack the network from outside. To mitigate attacks, it is useful to categorize the various types of attacks. The three major categories are reconnaissance, access, and DoS attacks. Reconnaissance is information gathering. Threat actors do unauthorized discovery and mapping of systems, services, or vulnerabilities. Recon attacks precede access or DoS attacks. Some of the techniques used include the following: performing an information query of a target, initiating a ping sweep of the target network, initiating a port scan of active IP addresses, running vulnerability scanners, and running exploitation tools. Access attacks exploit known vulnerabilities in authentication services, FTP services, and web services. These attacks include password attacks, spoofing attacks, trust exploitation attacks, port redirections, man-in-the-middle attacks, and buffer overflow attacks. Social engineering is an access attack that attempts to manipulate individuals into performing unsafe actions or divulging confidential information. These attacks include pretexting, phishing, spear phishing, spam, something for something, baiting, impersonation, tailgating, shoulder surfing, and dumpster diving.

* **Network Attacks – Denial of Service, Buffer Overflows, and Evasion**:

## Module 14: Common Threats and Attacks Quiz

1. Which is an example of social engineering?
   Topic 14.2.0 - A social engineer attempts to gain the confidence of an employee and convince that person to divulge confidential and sensitive information, such as usernames and passwords. DDoS attacks, pop-ups, and viruses are all examples of software based security threats, not social engineering.
   **an unidentified person claiming to be a technician collecting user information from employees**

2. What is a significant characteristic of virus malware?
   Topic 14.1.0 - A virus is malicious code that is attached to a legitimate program or executable file, and requires specific activation, which may include user actions or a time-based event. When activated, a virus can infect the files it has not yet infected, but does not automatically propagate itself to other systems. Self-propagation is a feature of worms. In addition to being distributed over the Internet, viruses are also spread by USB memory sticks, CDs, and DVDs.
   **A virus is triggered by an event on the host system.**

3. Which access attack method involves a software program that attempts to discover a system password by the use of an electronic dictionary? 
   Topic 14.3.0 - An access attack tries to affect services that affect entry into accounts, databases, and other sensitive information. Access attacks commonly involve a dictionary ths is used to guess a specific user password. A brute-force access attack would try to access an account via repeated attempts.
   **brute-force attack**
   
4. What is the purpose of a reconnaissance attack on a computer network?
   Topic 14.2.0 - Preventing users from accessing network resources is a denial of service attack. Being able to steal data from the network servers may be the objective after a reconnaissance attack gathers information about the target network and system. Redirecting data traffic so it can be monitored is a man-in-the middle attack.
   **to gather information about the target network and system.**

5. To which category of security attacks does man-in-the-middle belong?
   Topic 14.2.0 - With a man-in-the-middle attack, a threat actor is positioned in between two legitimate entities in order to read, modify, or redirect the data that passes between the two parties.
   **ACCESS**

6. What is the term used when a malicious party sends a fraudulent email disguised as being from a legitimate, trusted source?
   Topic 14.1.0 - Phishing is used by malicious parties who create fraudulent messages that attempt to trick a user into either sharing sensitive information or installing malware.
   **PHISHING**

7. What is the primary goal of a DoS attack?
   Topic 14.3.0 - A denial of service (DoS) attack attempts to overwhelm a system or process by sending large amounts of data or requests to the target. The goal is to keep the system so overwhelmed handling false requests that it is unable to respond to legitimate ones.
   to prevent the target server from being able to handle additional requests

8. What is the best description of Trojan horse malware?
   Topic 14.1.0 - The best description of Trojan horse malware, and what distinguishes it from viruses and worms, is that it appears as useful software but hides malicious code. Trojan horse malware may cause annoying computer problems, but can also cause fatal problems. Some Trojan horses may be distributed over the Internet, but they can also be distributed by USB memory sticks and other means. Specifically targeted Trojan horse malware can be some of the most difficult malware to detect.
   **it appears as useful software but hides malicious code.**

9.  Which tool is used to provide a list of open ports on network devices? 
    Topic 14.3.0 - The Nmap tool is a port scanner that is used to determine which ports are open on a particular network device. A port scanner is used before launching an attack.
    **NMAP**

10. When describing malware, what is a difference between a virus and a worm?
    Topic 14.1.0 - Malware can be classified as follows:

    Virus (self replicates by attaching to another program or file)
    Worm (replicates independently of another program)
    Trojan Horse (masquerades as a legitimate file or program)
    Rootkit (gains privileged access to a machine while concealing itself)
    Spyware (collects information from a target system)
    Adware (delivers advertisements with or without consent)
    Bot (waits for commands from the hacker)
    Ransomware (holds a computer system or data captive until payment is received)
    **a virus replicates itself by attaching to another file, whereas a worm can replicate itself independently.**

11. What is the main goal of using different evasion techniques by threat actors?
    Topic 14.3.0 - Many threat actors use stealthy evasion techniques to disguise an attack payload because  the malware and attack methods are most effective if they are undetected. The goal is to prevent detection by network and host defenses.
    **to prevent detection by network and host defenses.**

12. What is the purpose of a rootkit?
    Topic 14.3.0 - Malware can be classified as follows:

    Virus (self replicates by attaching to another program or file)
    Worm (replicates independently of another program)
    Trojan Horse (masquerades as a legitimate file or program)
    Rootkit (gains privileged access to a machine while concealing itself)
    Spyware (collects information from a target system)
    Adware (delivers advertisements with or without consent)
    Bot (waits for commands from the hacker)
    Ransomware (holds a computer system or data captive until payment is received)ent)
    **to gain privileged access to a device while concealing itself.**

13. In what way are zombies used in security attacks?
    Topic 14.3.0 - Zombies are infected computers that make up a botnet. The zombies are used to deploy a distributed denial of service (DDoS) attack.
    **they are infected machines that carry out a DDoS attack.**
   





  




