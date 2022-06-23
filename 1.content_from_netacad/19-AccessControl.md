# 19 Access control

## Introduction

How can you restrict access within your network? Will you allow all employees access to everything? Or will it be designed to allow users access based on their role in the company? How can you track what the user has accessed and what they did when they were logged in? Answer these questions and more by learning about access control concepts and AAA usage and operation.

## Access control concepts

### Communications Security: CIA

Information security deals with protecting information and information systems from unauthorized access, use, disclosure, disruption, modification, or destruction. the CIA triad consists of three components of information security:

* **Confidentiality**: Only authorized individuals, entities, or processes can access sensitive information.
* **Integrity**: This refers to the protection of data from unauthorized alteration.
* **Availability**: Authorized users must have uninterrupted access to the network resources and data that they require.

Network data can be encrypted (made unreadable to unauthorized users) using various cryptography applications. The conversation between two IP phone users can be encrypted. The files on a computer can also be encrypted. These are just a few examples. Cryptography can be used almost anywhere that there is data communication. In fact, the trend is toward all communication being encrypted.

### Zero Trust Security

Zero trust is a comprehensive approach to securing all access across networks, applications, and environments. **This approach helps secure access from users, end-user devices, APIs, IoT, microservices, containers, and more**. It protects an organization’s workforce, workloads, and the workplace. The principle of a zero trust approach is, **“never trust, always verify.”** Assume zero trust any time someone or something requests access to assets. **A zero trust security framework helps to prevent unauthorized access, contain breaches, and reduce the risk of an attacker's lateral movement through a network**.

Traditionally, the network perimeter, or edge, was the boundary between inside and outside, or trusted and untrusted. **In a Zero trust approach, any place at which an access control decision is required should be considered a perimeter**. This means that although a user or other entity may have successfully passed access control previously, they are not trusted to access another area or resource until they are authenticated. In some cases, users may be required to authenticate multiple times and in different ways, to gain access to different layers of the network.

The three pillars of zero trust are **workforce, workloads, and workplace**.

* **Zero Trust for the Workforce**: it consists of people who access work applications by using their personal or corporate-managed devices. It ensures only the right users and secure devices can access applications, regardless of location.

* **Zero Trust for Workloads**: it is concerned with applications that are running in the cloud, in data centers, and other virtualized environments that interact with one another. It focuses on secure access when an API, a microservice, or a container is accessing a database within an application.

* **Zero Trust for the Workplace**: it focuses on secure access for any and all devices, including on the internet of things (IoT), that connect to enterprise networks, such as user endpoints, physical and virtual servers, printers, cameras, HVAC systems, kiosks, infusion pumps, industrial control systems, and more.

### Access Control Models

An organization must implement proper access controls to protect its network resources, information system resources, and information. A security analyst should understand the different basic access control models to have a better understanding of how attackers can break the access controls.

|Access Control Models|Description|
|---------------------|-----------|
|Discretionary access control (DAC)| This is the least restrictive model and allows users to control access to their data as owners of that data. DAC may use ACLs or other methods to specify which users or groups of users have access to the information|
|Mandatory access control (MAC)| This applies the strictest access control and is typically used in military or mission critical applications. It assigns security level labels to information and enables users with access based on their security level clearance|
|Role-based access control (RBAC)| Access decisions are based on an individual’s roles and responsibilities within the organization. Different roles are assigned security privileges, and individuals are assigned to the RBAC profile for the role. Roles may include different positions, job classifications or groups of job classifications. Also known as a type of non-discretionary access control|
|Attribute-based access control (ABAC)| ABAC allows access based on attributes of the object (resource) to be accessed, the subject (user) accessing the resource, and environmental factors regarding how the object is to be accessed, such as time of day|
|Rule-based access control (RBAC)| Network security staff specify sets of rules regarding or conditions that are associated with access to data or systems. These rules may specify permitted or denied IP addresses, or certain protocols and other conditions. Also known as Rule Based RBAC|
|Time-based access control (TAC)|TAC Allows access to network resources based on time and day|

Another access control model is **the principle of least privilege**, which specifies a limited, as-needed approach to granting user and process access rights to specific information and tools. **The principle of least privilege states that users should be granted the minimum amount of access required to perform their work function**.

**A common exploit is known as privilege escalation**. In this exploit, vulnerabilities in servers or access control systems are exploited to grant an unauthorized user, or software process, higher levels of privilege than they should have. After the privilege is granted, the threat actor can access sensitive information or take control of a system.

## Check Your Understanding - Identify the Access Control Model

1. Which access control model is based on attributes of the object (resource) to be accessed, the subject (user) accessing the resource, and environmental factors regarding how the object is to be accessed, such as time of day? Attribute-based control allows access based on attributes of the object (resource) be accessed, the subject (user) accessing the resource, and environmental factors regarding how the object is to be accessed, such as time of day.
**attribute-based control.**

2. Which access control model is based on an individual’s roles and responsibilities within the organization? Non-discretionary access control allows access decisions based on an individual’s roles and responsibilities within the organization.
**non-discretionary access control.**

3. Which access control model applies the strictest access control and is typically used in military or mission critical applications? Mandatory access control applies the strictest access control and is typically used in military or mission critical applications. It assigns security level labels to information and enables users with access based on their security levels clearance.
**mandatory access control.**

## AAA Operation

A network must be designed to control who is allowed to connect to it and what they are allowed to do when they are connected. These design requirements are identified in the network security policy. The policy specifies how network administrators, corporate users, remote users, business partners, and clients access network resources. The network security policy can also mandate the implementation of an accounting system that tracks who logged in and when and what they did while logged in. Some compliance regulations may specify that access must be logged and the logs retained for a set period of time.

The Authentication, Authorization, and Accounting (AAA) protocol provides the necessary framework to enable scalable access security.

|AAA Component|Description|
|-------------|-----------|
|Authentication| Users and administrators must prove that they are who they say they are.     Authentication can be established using username and password combinations, challenge and response questions, token cards, and other methods. AAA authentication provides a centralized way to control access to the network|
|Authorization|After the user is authenticated, authorization services determine which resources the user can access and which operations the user is allowed to perform. An example is “User ‘student’ can access host server XYZ using SSH only.”|
|Accounting| Accounting records what the user does, including what is accessed, the amount of time the resource is accessed, and any changes that were made. Accounting keeps track of how network resources are used. An example is "User ‘student’ accessed host server XYZ using SSH for 15 minutes."|

### AAA Authentication

AAA Authentication can be used to authenticate users for administrative access or it can be used to authenticate users for remote network access. Cisco provides two common methods of implementing AAA services.

* Local AAA authentication: this method is sometimes known as self-contained authentication because it authenticates users against locally stored usernames and passwords.

1. The client establishes a connection with the router
2. The AAA router prompts the user for a username and password
3. The router authenticates the username and password using the local database and the user is provided access to the network based on information in the local database

* Server-based AAA authentication: this method authenticates against a central AAA server that contains the usernames and passwords for all users, as shown in the figure. Server-based AAA authentication is appropriate for medium-to-large networks.

1. The client establishes a connection with the router
2. The AAA router prompts the user for a username and password
3. The router authenticates the username and password using a AAA server
4. The user is provided acceess to the network based on information in the remote AAA server

Centralized AAA is more scalable and manageable than local AAA authentication and therefore, it is the preferred AAA implementation.

**A centralized AAA system may independently maintain databases for authentication, authorization, and accounting.** It can leverage Active Directory or Lightweight Directory Access Protocol (LDAP) for user authentication and group membership, while maintaining its own authorization and accounting databases. Devices communicate with the centralized AAA server using either the Remote Authentication Dial-In User Service (RADIUS) or Terminal Access Controller Access Control System (TACACS+) protocols.

|        |TACACS+|RADIUS|
|--------|-------|------|
|Functionality|It separates authentication, authorization, and accounting functions according to the AAA architecture. This allows modularity of the security server implementation|It combines authentication and authorization but separates accounting, which allows less flexibility in implementation than TACACS+|
|Standard|Mostly Cisco supported|Open/RFC standard|
|Transport|TCP port 49|UDP ports 1812 and 1813, or 1645 and 1646|
|Protocol CHAP|Bidirectional challenge and response as used in Challenge Handshake Authentication Protocol (CHAP)|Unidirectional challenge and response from the RADIUS security server to the RADIUS client|
|Confidentiality|Encrypts the entire body of the packet but leaves a standard TACACS+ header.|Encrypts only the password in the access-request packet from the client to the server. The remainder of the packet is unencrypted, leaving the username, authorized services, and accounting unprotected.|
|Customization|Provides authorization of router commands on a per-user or per-group basis|Has no option to authorize router commands on a per-user or per-group basis|
|Accounting|Limited|Extensive|

### AAA Accounting Logs

Centralized AAA also enables **the use of the Accounting method**. Accounting records from all devices are sent to centralized repositories, which simplifies auditing of user actions. **AAA Accounting collects and reports usage data in AAA logs**. **These logs are useful for security auditing**. The collected data might include the start and stop connection times, executed commands, number of packets, and number of bytes. One widely deployed use of accounting is to combine it with AAA authentication. This helps with managing access to internetworking devices by network administrative staff. Accounting provides more security than just authentication. The AAA servers keep a detailed log of exactly what the authenticated user does on the device, as shown in the figure. This includes all EXEC and configuration commands issued by the user. The log contains numerous data fields, including the username, the date and time, and the actual command that was entered by the user. This information is useful when troubleshooting devices. It also provides evidence against individuals who perform malicious actions.

1. When a user has been authenticated, the AAA accounting process generates a start message to begin the accounting process.
2. When the user finishes, a stop message is recorded and the accounting process ends.

|Type of Accounting Information|Description|
|------------------------------|-----------|
|Network Accounting|Network accounting captures information for all Point-to-Point Protocol (PPP) sessions, including packet and byte counts|
|Connection Accounting|Connection accounting captures information about all outbound connections that are made from the AAA client, such as by SSH|
|EXEC Accounting|EXEC accounting captures information about user EXEC terminal sessions (user shells) on the network access server, including username, date, start and stop times, and the access server IP address|
|System Accounting|System accounting captures information about all system-level events (for example, when the system reboots or when accounting is turned on or off)|
|Command Accounting|Command accounting captures information about the EXEC shell commands for a specified privilege level, as well as the date and time each command was executed, and the user who executed it|
|Resource Accounting|The Cisco implementation of AAA accounting captures “start” and “stop” record support for connections that have passed user authentication. The additional feature of generating “stop” records for connections that fail to authenticate as part of user authentication is also supported. Such records are necessary for users employing accounting records to manage and monitor their networks|

## Check Your Understanding - Identify the Characteristic of AAA

1. Records what the user does, including what is accessed, the amount of time the resource is accessed, and any changes that were made. **Accounting**
2. Uses a created set of attributes that describes the user’s access to the network. **Authorization**
3. Established using username and password combinations, challenge and response questions, token cards, and other methods. **Authentication**
4. Collects and reports usage data so that it can be employed for purposes such as auditing or billing. **Accounting**
5. Users and administrators must prove that they are who they say they are. **Authentication**
6. What a user can and cannot do on the network. **Authorization**
7. Which resources the user can access and which operations the user is allowed to perform. **Authorization**
8. Provides leverage against individuals who perform malicious actions. **Accounting**
9. A way to control who is permitted to access a network. **Authentication**

## Access Control Summary

**Access Control**: The CIA triad consists of the primary three components of information security: confidentiality, integrity, and availability. Network data can be encrypted (made unreadable to unauthorized users) using a variety of cryptography applications. The trend is that all data be encrypted. Zero trust is a comprehensive approach to securing all access across networks, applications, and environments. The principle of zero trust is “never trust, always verify”. Traditionally, the network perimeter, or edge, was the boundary between inside and outside, or trusted and untrusted. In a zero trust approach, any place at which an access control decision is required should be considered a perimeter. This means that although a user or other entity may have successfully passed access control previously, they are not trusted to access another area or resource until they are authenticated. The pillars of trust are zero trust for workforce, zero trust for workloads, and zero trust for workplace. Access control methods include discretionary access control (DAC), mandatory access control (MAC), role-based access control (RBAC), attribute-based control (ABAC), rule-based access (RBAC), and time-based access control (TAC). A common exploit is known as privilege escalation. In this exploit, vulnerabilities in servers or access control systems are exploited to grant access to an unauthorized user or software process.

**AAA Usage and Operation**: A network must be designed to control who is allowed to connect to it and what they are allowed to do when they are connected. These design requirements are identified in the network security policy. The policy can also mandate the implementation of an accounting system that tracks who logged and when and what they did when they were logged in. Authentication, Authorization, and Accounting (AAA) systems provide the necessary framework to enable scalable security. AAA authentication can be used to authenticate users for local access, or it can be used to authenticate users for remote network access. Cisco provides two common methods of implementing AAA services: Local AAA Authentication and Server-based AAA Authentication. Centralized AAA is more scalable and manageable than local AAA and is the preferred AAA implementation. A centralized AAA system can leverage Active Directory or Lightweight Directory Access Protocol (LDAP) for user authentication and group membership, while maintaining its own authorization and accounting databases. Devices communicate with the centralized AAA server using with the Remote Authentication Dial-In User Service (RADIUS) or Terminal Access Controller Access Control Systems (TACACS+) protocols. Centralized AAA also enables the use of the accounting method. AAA accounting collects and reports usage data in AAA logs. Various types of accounting information that can be collected are network accounting, connection accounting, EXEC accounting, system accounting, command accounting, and resource accounting.

## Module 19: Access Control Quiz

1. Which component of AAA is used to determine which resources a user can access and which operations the user is allowed to perform? Topic 19.2.0 - One of the components in AAA is authorization. After a user is authenticated through AAA, authorization services determine which resources the user can access and which operations the user is allowed to perform.
**Authorization**

2. What is the biggest issue with local implementation of AAA? Topic 19.2.0 - One of the purposes of AAA is to provide secure authentication to network devices. Local implementation does not use RADIUS or TACACS+ servers. It relies on a local database to authenticate all users. This can be a problem in a network that has many devices with hundreds of users or more. **​Local implementation does not scale well.**

3. A company is experiencing overwhelming visits to a main web server. The IT department is developing a plan to add a couple more web servers for load balancing and redundancy. Which requirement of information security is addressed by implementing the plan? Topic 19.1.0 - Availability ensures that network services are accessible and performing well under all conditions. By load balancing the traffic destined to the main web servers, in times of a huge volume of visits the systems will be well managed and serviced.
**Availability**

4. What is an example of privilege escalation attack? Topic 19.1.0 - With the privilege escalation exploit, vulnerabilities in servers or access control systems are exploited to grant an unauthorized user, or software process, higher levels of privilege than either should have. After the higher privilege is granted, the threat actor can access sensitive information or take control of a system.
**A threat actor performs an access attack and gains the administrator password.**

5. What is the principle of least privilege access control model? Topic 19.1.0 - The principle of least privilege is an access control model that specifies a limited and as-needed approach to user access to data.
**Users are granted rights on an as-needed approach.**

6. A server log includes this entry: User student accessed host server ABC using Telnet yesterday for 10 minutes. What type of log entry is this? Topic 19.2.0 - Accounting records what users do and when they do it, including what is accessed, the amount of time the resource is accessed, and any changes that were made. Accounting keeps track of how network resources are used. 
**Accounting**

7. Which objective of secure communications is achieved by encrypting data? Topic 19.1.0 - When data is encrypted, it is scrambled to keep the data private and confidential so that only authorized recipients can read the message. A hash function is another way of providing confidentiality.
**Confidentiality.**

8. What are three access control security services? (Choose three.) Topic 19.2.0 - This question refers to AAA authentication, authorization, and accountability.
**Authentication, accounting, authorization**

9. Which access control model allows users to control access to data as an owner of that data?Topic 19.1.0 - In the discretionary access control (DAC) model, users can control access to data as owners of the data.
**Discretionary access control.** 

10. Which two protocols are used to provide server-based AAA authentication? (Choose two.) Topic 19.2.0 - Server-based AAA authentication uses an external TACACS or RADIUS authentication server to maintain a username and password database. When a client establishes a connection with an AAA enabled device, the device authenticates the client by querying the authentication servers.
**RADIUS, TACACS+**

11. What three items are components of the CIA triad? (Choose three.) Topic 19.1.0 - The CIA triad contains three components: confidentiality, integrity, and availability. It is a guideline for information security for an organization.
**Integrity, availability, confidentiality.**

12. Which type of access control applies the strictest access control and is commonly used in military or mission critical applications? Topic 19.1.0 - Access control models are used to define the access controls implemented to protect corporate IT resources. The different types of access control models are as follows:

    Mandatory access control (MAC) – The strictest access control that is typically used in military or mission critical applications.
    Discretionary access control (DAC) – Allows users to control access to their data as owners of that data. Access control lists (ACLs) or other security measures may be used to specify who else may have access to the information.
    Non-discretionary access control – Also known as role-based access control (RBAC). Allows access based on the role and responsibilities of the individual within the organization.
    Attribute-based access control (ABAC) – Allows access based on the attributes of the resource to be accessed, the user accessing the resource, and the environmental factors such as the time of day. 
**Mandatory access control.**