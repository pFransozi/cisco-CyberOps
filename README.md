# CyberOps Associate

In this repository there are topics about cisco cyberops associate certificate, such as: contents from Cisco NetAcad, LinkedIn course called **CyberOps Associate: Prepare for the Cisco Cybersecurity Operations Fundamentals (200-201 CBROPS) Exam**, and books that cover cyberops certificate. 

**The purpose of this content is only educational**

About materials from netacad, see [NetAcad](1.content_from_netacad/)
About materials from inLearning, see [InLearning](2.content_from_inLearning/)
About books, see [books](books/)
About wireshark, see [wireshark](3.wireshark/)

The Understanding Cisco Cybersecurity Operations Fundamentals v1.0 (200-201) is related to the Cisco Certified CyberOps Associate
certification. It tests the knowledge and skills related to security concepts, security monitoring host-based analysis, network intrusion analysis, and security policies and procedures.

There are five main topics:

1. **20% Security Concepts**
    * Describe the CIA triad
    * Compare security deployments
        * Network, endpoint, and application security systems
        * Agentless and agent-based protections
        * Legacy antivirus and antimalware
        * SIEM, SOAR, and log management
    * Describe security terms
        * Threat intelligence (TI)
        * Threat hunting
        * Malware analysis
        * Threat actor
        * Run book automation (RBA)
        * Reverse engineering
        * Sliding window anomaly detection
        * Principle of least privilege
        * Zero trust
        * Threat intelligence platform (TIP)
    * Compare security concepts
        * Risk (risk scoring/risk weighting, risk reduction, risk assessment)
        * Threat
        * Vulnerability
        * Exploit
    * Describe the principles of the defense-in-depth strategy
    * Compare access control models
        * Discretionary access control
        * Mandatory access control
        * Nondiscretionary access control
        * Authentication, authorization, accounting
        * Rule-based access control
        * Time-based access control
        * Role-based access control
    * Describe terms as defined in CVSS
        * Attack vector
        * Attack complexity
        * Privileges required
        * User interaction
        * Scope
    * Identify the challenges of data visibility (network, host, and cloud) in detection
    * Identify potential data loss from provided traffic profiles
    * Interpret the 5-tuple approach to isolate a compromised host in a grouped set of logs
    * Compare rule-based detection vs. behavioral and statistical detection
2. **25% Security Monitoring**
    * Compare attack surface and vulnerability
    * Identify the types of data provided by these technologies
        * TCP dump
        * NetFlow
        * Next-gen firewall
        * Traditional stateful firewall
        * Application visibility and control
        * Web content filtering
        * Email content filtering
    * Describe the impact of these technologies on data visibility
        * Access control list
        * NAT/PAT
        * Tunneling
        * TOR
        * Encryption
        * P2P
        * Encapsulation
        * Load balancing
    * Describe the uses of these data types in security monitoring
        * Full packet capture
        * Session data
        * Transaction data
        * Statistical data
        * Metadata
        * Alert data
    * Describe network attacks, such as protocol-based, denial of service, distributed denial of service, and man-in-the-middle
    * Describe web application attacks, such as SQL injection, command injections, and cross-site scripting
    * Describe social engineering attacks
    * Describe endpoint-based attacks, such as buffer overflows, command and control (C2), malware, and ransomware
    * Describe evasion and obfuscation techniques, such as tunneling, encryption, and proxies
    * Describe the impact of certificates on security (includes PKI, public/private crossing the network, asymmetric/symmetric)
    * Identify the certificate components in a given scenario
        * Cipher-suite
        * X.509 certificates
        * Key exchange
        * Protocol version
        PKCS
* **20% Host-based analysis**
    * Describe the functionality of these endpoint technologies in regard to security monitoring
        * Host-based intrusion detection
        * Antimalware and antivirus
        * Host-based firewall
        * Application-level allow listing/block listing
        * Systems-based sandboxing (such as Chrome, Java, Adobe Reader)
    * Identify components of an operating system (such as Windows and Linux) in a given scenario
    * Describe the role of attribution in an investigation
        * Assets
        * Threat actor
        * Indicators of compromise
        * Indicators of attack
        * Chain of custody
    * Identify type of evidence used based on provided logs
        * Best evidence
        * Corroborative evidence
        * Indirect evidence
    * Compare tampered and untampered disk image
    * Interpret operating system, application, or command line logs to identify an event
    * Interpret the output report of a malware analysis tool (such as a detonation chamber or sandbox)
        * Hashes
        * URLs
        * Systems, events, and networking
* **20% Network Intrusion Analysis**
    * Map the provided events to source technologies
        * IDS/IPS
        * Firewall
        * Network application control
        * Proxy logs
        * Antivirus
        * Transaction data (NetFlow)
    * Compare impact and no impact for these items
        * False positive
        * False negative
        * True positive
        * True negative
        * Benign
    * Compare deep packet inspection with packet filtering and stateful firewall operation
    * Compare inline traffic interrogation and taps or traffic monitoring
    * Compare the characteristics of data obtained from taps or traffic monitoring and transactional data (NetFlow) in the analysis of network traffic
    * Extract files from a TCP stream when given a PCAP file and Wireshark
    * Identify key elements in an intrusion from a given PCAP file
        * Source address
        * Destination address
        * Source port
        * Destination port
        * Protocols
        * Payloads
    * Interpret the fields in protocol headers as related to intrusion analysis
        * Ethernet frame
        * IPv4
        * IPv6
        * TCP
        * UDP
        * ICMP
        * DNS
        * SMTP/POP3/IMAP
        * HTTP/HTTPS/HTTP2
        * ARP
    * Interpret common artifact elements from an event to identify an alert
        * IP address (source / destination)
        * Client and server port identity
        * Process (file or registry)
        * System (API calls)
        * Hashes
        * URI / URL
    * Interpret basic regular expressions
* **15% Security Policies and Procedures**
    * Describe management concepts
        * Asset management
        * Configuration management
        * Mobile device management
        * Patch management
        * Vulnerability management
    * Describe the elements in an incident response plan as stated in NIST.SP800-61
    * Apply the incident handling process (such as NIST.SP800-61) to an event
    * Map elements to these steps of analysis based on the NIST.SP800-61
        * Preparation
        * Detection and analysis
        * Containment, eradication, and recovery
        * Post-incident analysis (lessons learned)
    * Map the organization stakeholders against the NIST IR categories (CMMC, NIST.SP800-61)
        * Preparation
        * Detection and analysis
        * Containment, eradication, and recovery
        * Post-incident analysis (lessons learned)
    * Describe concepts as documented in NIST.SP800-86
        * Evidence collection order
        * Data integrity
        * Data preservation
        * Volatile data collection
    * Identify these elements used for network profiling
        * Total throughput
        * Session duration
        * Ports used
        * Critical asset address space
    * Identify these elements used for server profiling
        * Listening ports
        * Logged in users/service accounts
        * Running processes
        * Running tasks
        * Applications
    * Identify protected data in a network
        * PII
        * PSI
        * PHI
        * Intellectual property
    * Classify intrusion events into categories as defined by security models, such as Cyber Kill Chain Model and Diamond Model of Intrusion
    * Describe the relationship of SOC metrics to scope analysis (time to detect, time to contain, time to respond, time to control)