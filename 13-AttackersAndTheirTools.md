# 13 Attacker and their tools

Who is attacking our network and why?

## Who is Attacking Our Network?

### Threat, Vulnerability, and Risk

Basic terms

| Term | Explanation |
|------|-------------|
|Threat|A potential danger to an asset such as data or the network itself|
|Vulnerability|A weakness in a system or its design that could be exploited by a threat|
|Attack surface|An attack surface is the total sum of the vulnerabilities in a given system that are accessible to an attacker. The attack surface describes different points where an attacker could get into a system, and where they could get data out of the system. For example, your operating system and web browser could both need security patches. They are each vulnerable to attacks and are exposed on the network or the internet. Together, they create an attack surface that the threat actor can exploit|
|Exploit|The mechanism that is used to leverage a vulnerability to compromise an asset. Exploits may be remote or local. A remote exploit is one that works over the network without any prior access to the target system. The attacker does not need an account in the end system to exploit the vulnerability. In a local exploit, the threat actor has some type of user or administrative access to the end system. A local exploit does not necessarily mean that the attacker has physical access to the end system.|
|Risk|The likelihood that a particular threat will exploit a particular vulnerability of an asset and result in an undesirable consequence|
|Countermeasure|The actions that are taken to protect assets by mitigating a threat or reducing risk|
|Impact|The potential damage to the organization that is caused by the threat|

Risk management is the process that balances the operational costs of providing protective measures with the gains achieved by protecting the asset. There are four common ways to manage risk:

|Risk Management Strategy|Explanation|
|------------------------|-----------|
|Risk acceptance|This is when the cost of risk management options outweighs the cost of the risk itself. The risk is accepted, and no action is taken|
|Risk avoidance|This means avoiding any exposure to the risk by eliminating the activity or device that presents the risk. By eliminating an activity to avoid risk, any benefits that are possible from the activity are also lost|
|Risk reduction|This reduces exposure to risk or reducing the impact of risk by taking action to decrease the risk. It is the most commonly used risk mitigation strategy. This strategy requires careful evaluation of the costs of loss, the mitigation strategy, and the benefits gained from the operation or activity that is at risk|
|Risk transfer|Some or all of the risk is transferred to a willing third party such as an insurance company|

### Hacker vs. Threat Actor

1. White hat hackers are ethical hackers who use their programming skills for good, ethical, and legal purposes. They may perform network penetration tests in an attempt to compromise networks and systems by using their knowledge of computer security systems to discover network vulnerabilities. Security vulnerabilities are reported to developers and security personnel who attempt to fix the vulnerability before it can be exploited. Some organizations award prizes or bounties to white hat hackers when they provide information that helps to identify vulnerabilities;
2. Gray hat hackers are individuals who commit crimes and do arguably unethical things, but not for personal gain or to cause damage. An example would be someone who compromises a network without permission and the discloses the vulnerability publicly. Grey hat hackers may disclose a vulnerability to the affected organization after having compromised their network. This allows the organization to fix the problem.
3. Black hat hackers are unethical criminals who violate computer and network security for personal gain, or for malicious reasons, such as attacking networks. Black hat hackers exploit vulnerabilities to compromise computer and network systems.

Good or bad, hacking is an important aspect of network security. **The term threat actor is used when referring to those individuals or groups that could be classified as gray or black hat hackers**.

### Evolution of Threat Actors

* Script kiddies emerged in the 1990s and refers to teenagers or inexperienced threat actors running existing scripts, tools, and exploits, to cause harm, but typically not for profit.
* Vulnerability brokers typically refers to grey hat hackers who attempt to discover exploits and report them to vendors, sometimes for prizes or rewards.
* Hacktivists is a term that refers to grey hat hackers who rally and protest against different political and social ideas. Hacktivists publicly protest against organizations or governments by posting articles, videos, leaking sensitive information, and performing distributed denial of service (DDoS) attacks.
* Cybercriminal is a term for black hat hackers who are either self-employed or working for large cybercrime organizations. Each year, cyber criminals are responsible for stealing billions of dollars from consumers and businesses.
* State-Sponsored hackers are threat actors who steal government secrets, gather intelligence, and sabotage networks of foreign governments, terrorist groups, and corporations. Most countries in the world participate to some degree in state-sponsored hacking. Depending on a person’s perspective, these are either white hat or black hat hackers.

### Cybercriminals

Cybercriminals are threat actors who are motivated to make money using any means necessary. While sometimes cybercriminals work independently, they are more often financed and sponsored by criminal organizations. It is estimated that globally, cybercriminals steal billions of dollars from consumers and businesses every year. Cybercriminals operate in an underground economy where they buy, sell, and trade exploits and tools. They also buy and sell the personal information and intellectual property that they steal from victims. Cybercriminals target small businesses and consumers, as well as large enterprises and industries.

### Cybersecurity Tasks

To make the internet and networks safer and more secure, we must all develop good cybersecurity awareness. Cybersecurity is a shared responsibility which all users must practice. For example, we must report cybercrime to the appropriate authorities, be aware of potential threats in email and the web, and guard important information from theft.

### Cyber Threat Indicators

Many network attacks can be prevented by sharing information **about indicators of compromise (IOC)**. Each attack has unique identifiable attributes. **IOCs can be features that identify malware files, IP addresses of servers that are used in attacks, filenames, and characteristic changes made to end system software, among others**.

**Indicators of attack (IOA)** **focus more on the motivation behind an attack and the potential means by which threat actors have**, or will, **compromise vulnerabilities to gain access to assets**. IOAs are concerned with the strategies that are used by attackers. For this reason, rather than informing response to a single threat, IOAs can help generate a proactive security approach. This is because strategies can be reused in multiple contexts and multiple attacks. Defending against a strategy can therefore prevent future attacks that utilize the same, or similar strategy.

### Threat Sharing and Building Cybersecurity Awareness

Governments are now actively promoting cybersecurity. For instance, the US Cybersecurity Infrastructure and Security Agency (CISA) is leading efforts to automate the sharing of cybersecurity information with public and private organizations at no cost. CISA use a system called Automated Indicator Sharing (AIS). AIS enables the sharing of attack indicators between the US government and the private sector as soon as threats are verified. CISA offers many resources that help to limit the size of the United States attack surface. The CISA and the National Cyber Security Alliance (NCSA) promote cybersecurity to all users. For example, they have an annual campaign in every October called “National Cybersecurity Awareness Month” (NCASM). This campaign was developed to promote and raise awareness about cybersecurity.

The theme for the NCASM for 2019 was “Own IT. Secure IT. Protect IT.” This campaign encouraged all citizens to be safer and more personally accountable for using security best practices online. The campaign provides material on a wide variety of security topics including:

    Social media safety
    Updating privacy settings
    Awareness of device app security
    Keeping software up-to-date
    Safe online shopping
    Wi-Fi safety
    Protecting customer data

### Check Your Understanding – What Color is my Hat?

I hacked into ATM machines without the manufacturer's authorization and discovered several vulnerabilities. I then contacted the ATM manufacturer to share my findings with them. **Gray Hat**

I secretly installed a debit card skimmer device on an ATM machine. A few days later, I retrieved it and it had captured the account numbers and pins numbers of over 1000 people. I then proceeded to transfer money from their accounts to an offshore bank account. **Black hat**

My job is to identify weaknesses in the computer system in my company. **White hat**

I used malware to compromise several corporate systems to steal credit card information and sold that information to the highest bidder. **Black hat**

During my research for security exploits, I stumbled across a security vulnerability on a corporate network that I am authorized to access. **White hat**

While I was searching for security vulnerabilities, I gained unauthorized access to a company’s network and left the message “Your security is flawed”. **Gray hat**

I am working with technology companies to fix a flaw with DNS. **White hat**


## Threat Actor Tools

### Introduction of Attack Tools

To exploit a vulnerability, a threat actor must have a technique or tool. Over the years, attack tools have become more sophisticated, and highly automated. These new tools require less technical knowledge to implement. 

### Evolution of Security Tools

Ethical hacking involves using many different types of tools to test the network and end devices. To validate the security of a network and its systems, many network penetration testing tools have been developed. However, many of these tools can also be used by threat actors for exploitation. Threat actors have also created various hacking tools. These tools are explicitly written for nefarious reasons. Cybersecurity personnel must also know how to use these tools when performing network penetration tests. Explore the categories of common network penetration testing tools. Notice how some tools are used by white hats and black hats. Keep in mind that the list is not exhaustive as new tools are continually being developed.

|Categories of Tools|Description|
|-------------------|-----------|
|password crackers  |Passwords are the most vulnerable security threat. Password cracking tools are often referred to as password recovery tools and can be used to crack or recover the password. This is accomplished either by removing the original password, after bypassing the data encryption, or by outright discovery of the password. Password crackers repeatedly make guesses in order to crack the password and access the system. Examples of password cracking tools include John the Ripper, Ophcrack, L0phtCrack, THC Hydra, RainbowCrack, and Medusa.|
|wireless hacking tools|Wireless networks are more susceptible to network security threats. Wireless hacking tools are used to intentionally hack into a wireless network to detect security vulnerabilities. Examples of wireless hacking tools include Aircrack-ng, Kismet, InSSIDer, KisMAC, Firesheep, and NetStumbler|
|network scanning and hacking tools|Network scanning tools are used to probe network devices, servers, and hosts for open TCP or UDP ports. Examples of scanning tools include Nmap, SuperScan, Angry IP Scanner, and NetScanTools|
|packet crafting tools|Packet crafting tools are used to probe and test a firewall’s robustness using specially crafted forged packets. Examples of such tools include Hping, Scapy, Socat, Yersinia, Netcat, Nping, and Nemesis|
|packet sniffers|Packet sniffers tools are used to capture and analyze packets within traditional Ethernet LANs or WLANs. Tools include Wireshark, Tcpdump, Ettercap, Dsniff, EtherApe, Paros, Fiddler, Ratproxy, and SSLstrip|
|rootkit detectors|A rootkit detector is a directory and file integrity checker used by white hats to detect installed root kits. Example tools include AIDE, Netfilter, and PF: OpenBSD Packet Filter|
|fuzzers to search vulnerabilities |Fuzzers are tools used by threat actors when attempting to discover a computer system’s security vulnerabilities. Examples of fuzzers include Skipfish, Wapiti, and W3af|
|forensic tools|White hat hackers use forensic tools to sniff out any trace of evidence existing in a particular computer system. Example of tools include Sleuth Kit, Helix, Maltego, and Encase|
|debuggers|Debugger tools are used by black hats to reverse engineer binary files when writing exploits. They are also used by white hats when analyzing malware. Debugging tools include GDB, WinDbg, IDA Pro, and Immunity Debugger|
|hacking operating systems|Hacking operating systems are specially designed operating systems preloaded with tools and technologies optimized for hacking. Examples of specially designed hacking operating systems include Kali Linux, SELinux, Knoppix, Parrot OS, and BackBox Linux|
|encryption tools|These tools safeguard the contents of an organization’s data when it is stored or transmitted. Encryption tools use algorithm schemes to encode the data to prevent unauthorized access to the data. Examples of these tools include VeraCrypt, CipherShed, Open SSH, OpenSSL, OpenVPN, and Stunnel|
|vulnerability exploitation tools|These tools identify whether a remote host is vulnerable to a security attack. Examples of vulnerability exploitation tools include Metasploit, Core Impact, Sqlmap, Social Engineer Tool Kit, and Netsparker|
|vulnerability scanners|These tools scan a network or system to identify open ports. They can also be used to scan for known vulnerabilities and scan VMs, BYOD devices, and client databases. Examples of these tools include Nipper, Securia PSI, Core Impact, Nessus, SAINT, and Open VAS|

### Categories of Attacks

|Category of Attack|Description|
|------------------|-----------|
|eavesdropping attack|An eavesdropping attack is when a threat actor captures and listens to network traffic. This attack is also referred to as sniffing or snooping|
|data modification attack|Data modification attacks occur when a threat actor has captured enterprise traffic and has altered the data in the packets without the knowledge of the sender or receiver|
|IP address spoofing attack|An IP address spoofing attack is when a threat actor constructs an IP packet that appears to originate from a valid address inside the corporate intranet|
|password-based attacks|Password-based attacks occur when a threat actor obtains the credentials for a valid user account. Threat actors then use that account to obtain lists of other users and network information. They could also change server and network configurations, and modify, reroute, or delete data|
|denial-of-service (DoS) attack|A DoS attack prevents normal use of a computer or network by valid users. After gaining access to a network, a DoS attack can crash applications or network services. A DoS attack can also flood a computer or the entire network with traffic until a shutdown occurs because of the overload. A DoS attack can also block traffic, which results in a loss of access to network resources by authorized users|
|man-in-the-middle attack (MiTM)|A MiTM attack occurs when threat actors have positioned themselves between a source and destination. They can now actively monitor, capture, and control the communication transparently|
|compromised key attack|A compromised-key attack occurs when a threat actor obtains a secret key. This is referred to as a compromised key. A compromised key can be used to gain access to a secured communication without the sender or receiver being aware of the attack|
|sniffer attack|A sniffer is an application or device that can read, monitor, and capture network data exchanges and read network packets. If the packets are not encrypted, a sniffer provides a full view of the data inside the packet. Even encapsulated (tunneled) packets can be broken open and read unless they are encrypted and the threat actor does not have access to the key|

### Check Your Understanding - Classify Cyber Attacks

1. Hackers have gained access to account information and can now login into a system with the same rights as authorized users. What type of attack is this? **Password-based attack**
2. In what type of attack can threat actors change the data in packets without the knowledge of the sender or receiver? **data modification attack**
3. Threat actors have positioned themselves between a source and destination to monitor, capture, and control communications without the knowledge of network users. What type of attack is this? **MiTM**
4. A threat actor has gained access to encryption keys that will permit them to read confidential information. What type of attack is this? compromised key attack
5. In what type of attack does a threat attacker attach to the network and read communications from network users? **eavesdropping attack**
6. A threat actor constructs IP packets that appear to come from a valid source within the corporate network. What type of attack is this? **IP address attack**
7. What type of attack prevents the normal use of a computer or network by valid users? **DoS**

## Attackers and Their Tools Summary

* **Who is Attacking Our Network?** Understanding network security requires you to understand the following terms: threat, vulnerability, attack surface, exploit, and risk. Risk management is the process that balances the operational costs of providing protective measures with the gains achieved by protecting the asset. Four common ways to manage risk are risk acceptance, risk avoidance, risk reduction, and risk transfer. Hacker is a term used to describe a threat actor. White hat hackers are ethical hackers using their skills for good, ethical, and legal purposes. Grey hat hackers are individuals who commit crimes and do unethical things, but not for personal gain or to cause damage. Black hat hackers are criminals who violate computer and network security for personal gain, or for malicious reasons, such as attacking networks. Threat actors include script kiddies, vulnerability brokers, hacktivists, cybercriminals, and state-sponsored hackers. Many network attacks can be prevented by sharing information about indicators of compromise (IOC). Many governments are promoting cybersecurity. CISA and NCSA are examples of such organizations.
* Introduction of Attack Tools: Threat actors use a technique or tool. Attack tools have become more sophisticated, and highly automated. Many of the tools are Linux or UNIX based and a knowledge of these are useful to a cybersecurity professional. Tools include password crackers, wireless hacking tools, network security scanning and hacking tools, packet crafting tools, packet crafting tools, packet sniffers, rootkit detectors, fuzzers to search vulnerabilities, forensic tools, debuggers, hacking operating systems, encryption tools, vulnerability exploitation tools, and vulnerability scanners. Categories of attacks include eavesdropping attacks, data modification attacks, IP address spoofing attacks, password-based attacks, denial-of-service attacks, man-in the-middle attacks, compromised key attacks, and sniffer attacks.

## Module 13: Attackers and Their Tools Quiz

1. **What is an example of "hacktivism"?**
   Topic 13.1.0 - Hacktivism is a term used to describe cyberattacks carried out by people who are considered political or ideological extremists. Hacktivists attack people or organizations that they believe are enemies to the hacktivist agenda.
   **A group of environmentalists launch a denial of service attack against an oil company that is responsible for a large oil spill.**

2. **Which statement describes cybersecurity?**
   Topic 13.1.0 - Cybersecurity is the ongoing effort to protect Internet-connected network systems and all of the data associated with the systems from unauthorized use or harm.
   **It is an ongoing effort to protect internet-connected systems and the data associated with those systems from unauthorized use or harm.**

3. **What focus describes a characteristic of an indicator of attack (IOA)?**
   Topic 13.1.0 - Indicators of attack (IOA) focus more on the motivation behind an attack and the potential means by which threat actors have, or will, compromise vulnerabilities to gain access to assets. IOAs are concerned with the strategies that are used by attackers and can help generate a proactive security approach.
   It focuses more on the motivation behind an attack and the means used to compromise vulnerabilities to gain access to assets.

4. **What is the motivation of a white hat attacker?**
   Topic 13.1.0 - White hat attackers break into networks or computer systems in order to discover weaknesses for the purpose of improving the security of these systems. These break-ins are done with permission from the owner or the organization. Any results are reported back to the owner or the organization.
   **discovering weaknesses of networks and systems to improve the security level of these systems.**

5. **Which risk management plan involves discontinuing an activity that creates a risk?**
   Topic 13.1.0 - During a risk assessment it may be determined that an activity involves more risk than benefit. In such a situation an organization may decide to avoid the risk altogether by discontinuing the activity. This is known as risk avoidance.
   **risk avoidance**

6. **Which type of network threat is intended to prevent authorized users from accessing resources?**
   Topic 13.2.0 - Network reconnaissance attacks involve the unauthorized discovery and mapping of the network and network systems. Access attacks and trust exploitation involve unauthorized manipulation of data and access to systems or user privileges. DoS, or Denial of Service attacks, are intended to prevent legitimate users and devices from accessing network resources.
   **DoS**

7. **What security tool allows a threat actor to hack into a wireless network and detect security vulnerabilities?**
   Topic 13.2.0 - Aircrack-ng, Kismet, InSSIDer, KisMAC, Firesheep, and NetStumbler are examples of tools used to hack into a wireless network.
   **KisMac**

8. **Which statement describes the term attack surface?**
   Topic 13.1.0 - An attack surface is the total sum of the vulnerabilities in a system that is accessible to an attacker. The attack surface can consist of open ports on servers or hosts, software that runs on Internet-facing servers, wireless network protocols, and even users.
   **It is the total sum of vulnerabilities in a system that is accessible to an attacker.**

9.  **Which risk management strategy requires careful evaluation of the costs of loss, the mitigation strategy, and the benefits gained from the operation or activity that is at risk?**
    Topic 13.1.0 - Risk reduction strategy reduces exposure to risk or reduces the impact of risk by taking action to decrease the risk. It is the most commonly used risk mitigation strategy. This strategy requires careful evaluation of the costs of loss, the mitigation strategy, and the benefits gained from the operation or activity that is at risk.

10. **What characteristic describes script kiddies?**
    Topic 13.1.0 - Script kiddies refers to teenagers or inexperienced threat actors running existing scripts, tools, and exploits, to cause harm, but typically not for profit.
    **inexperienced threat actors running existing scripts, tools, and exploits, to cause harm, but typically not for profit.**

11. **What characteristic describes a gray hat hacker?**
    Topic 13.1.0 - Gray hat hackers are individuals who commit crimes and do arguably unethical things, but not for personal gain or to cause damage.
    **individuals who commit cyber crimes but not for personal gain or to cause damage.**

12. **A company has contracted with a network security firm to help identify the vulnerabilities of the corporate network. The firm sends a team to perform penetration tests to the company network. Why would the team use forensic tools?**
    Topic 13.2.0 - Ethical hacking involves using many different types of tools to test the network and end devices. To validate the security of a network and its systems, many network penetration testing tools have been developed. These tools are used to test the vulnerability and susceptibility of networks to be cracked, probed, hacked, captured, and hijacked. Many of the tools are Linux or Linux based and can be used by both white and black hats.
    **to detect any evidence of a hack or malware in a computer or network.**

13. **A company has contracted with a network security firm to help identify the vulnerabilities of the corporate network. The firm sends a team to perform penetration tests to the company network. Why would the team use applications such as Nmap, SuperScan, and Angry IP Scanner?**
    Topic 13.2.0 - Ethical hacking involves using many different types of tools to test the network and end devices. Network scanning tools are used to probe network devices, servers, and hosts for open TCP or UDP ports. Examples of scanning tools include Nmap, SuperScan, Angry IP Scanner, and NetScanTools.
    **to probe network devices, servers, and hosts for open TCP or UDP ports.**