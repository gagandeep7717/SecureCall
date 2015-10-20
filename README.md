# SecureCall
###**Peer to peer voice communication using ZRTP**

Project Members: 	Gagandeep Singh Randhawa and Aniket Nade

####Problem Statement
VoIP Strategy has been around for a while, using the data connectivity to transmit and receive voice. VoIP is made practical on mobiles by the data speed offered by mobile networks recently. But security in VoIP remains of top concern as voice packets are delivered over public internet, Also the confidentiality is at risk as it uses transparent IP protocol suite. Using Cryptographic key exchange to encrypt media stream is quite difficult task. Voice communications over VoIP are vulnerable to man in the middle attack. There is a need of stronger mechanism that protects voice packets from such vulnerabilities.

####Proposed solution
We propose to make use of Pretty Good Privacy (PGP) as strong cryptography protocol for voice communication. PGP is a scheme that provides data encryption and decryption with cryptographic privacy and authentication. It is often used for encrypting and decrypting e-mails, files and texts. This will prevent the adversary from intercepting the communication being held over the internet. We aim to establish an end to end connection between two parties. We are planning to involve android smartphones as the end points. VoIP simulation will be done via Asterisk (An Open Source VoIP simulator)[5].
Following are the protocols to be used in implementation:

**ZRTP**: Zimmerman, Real-time Transport Protocol (ZRTP) is a cryptographic key-agreement protocol to negotiate the keys for encryption between two end points in a Voice over Internet Protocol (VoIP) phone telephony call based on the Real-time Transport Protocol. It uses Diffie–Hellman key exchange and the Secure Real-time Transport Protocol (SRTP) for encryption[3].

**SIP**: The Session Initiation Protocol (SIP) is a communications protocol for signaling and controlling multimedia communication sessions. SIP is commonly used in Internet telephony for voice and video calls, as well as instant messaging all over Internet Protocol (IP) networks[2].

**H323**: H323 is a protocol Standardized by the International Telecommunication Union (ITU), H323 is a signaling approach used for the deployment of VoIP systems. This protocol defines call setup messages and procedures used to establish a call, as well as messages and procedures used for user’s registration. It also defines security profiles such as authentication, message integrity, signature security, and voice encryption[4].

####Details of implementation
**Platform**: Android

**Programming Language**: Java

**Components Involved**: 
-	VoIP simulation tool (Asterisk)
-	Wireshark
-	PGP libraries provided by OpenPGP

####**Timeline of Work**
1.	**14th September - 27th September**
 - 1.1. Understanding Mobile VoIP implementation
 - 1.2. Potential vulnerabilities in VoIP systems
2.  **28th September - 20th October**
 - 2.1. Understanding Pretty Good Privacy protocol
 - 2.2. Study implementation of PGP in java
 - 2.3. Studying key exchange mechanisms
3.	**21st October - 20th November**
 - 3.1.	Integrating PGP into VoIP
 - 3.2. VoIP simulation using Asterisk
 - 3.3.	Performance analysis of the system.


###**Milestone 1.1**
- **Understanding VoIP implementation**

We are using PBX service provided by [PBXes.com](https://www2.pbxes.com/). 
A **private branch exchange (PBX)** is a switching system that serves a private organization and provides intercommunication between two end points. 
The aspect of a PBX permits the shared use of these lines between all stations in the organization. 
Each PBX-connected station, an Android Phone in our case, is often referred to as an extension and has a designated extension telephone number that may or may not be mapped automatically to the numbering plan of the central office and the telephone number block allocated to the PBX.[7]
Since we are using a free account of PBX, it lets us create only 5 extensions. We have created two right now for testing purposes and other extensions can be added later as required. The number of extensions can be increased by purchasing premium account provided by PBXes.com.

Functionally, the PBX performs four main call processing duties:[7]

1. Establishing connections (circuits) between the telephone sets of two users (e.g. mapping a dialed number to a physical phone, ensuring the phone isn't already busy)
2. Maintaining such connections as long as the users require them (i.e. channelling voice signals between the users)
3. Disconnecting those connections as per the user's requirement
4. Providing information for accounting purposes (e.g. metering calls)

Each PBX Account has following characteristics:

1. **Extensions** - An extension is just the definition of a classic SIP (VOIP) telephone line/number. SIP extensions are normally used to register SIP devices to, like SIP phones, softphones or ADSL modems having SIP capabilities. Unlike classic extensions, SIP extensions can be used to place calls too[8].
2. 	**Trunks** - Trunks are definitions of the SIP providers you want to use for receiving inbound calls and/or placing outbound calls. Inbound calls are routed to extensions using inbound routes, and outbound calls are routed to a trunk using the outbound routes. For receiving inbound calls it is necessary to register to the SIP provider[8].
Note: Our major focus is to implement a SIP client on Android smartphone.


####**References**

1. Alan Johnston and Davind Piscitello. Understanding Voice Over IP Security. Artech House Publishers.
 
2. Alan Johnston. Sip: Understanding the Session Initiation Protocol. Artech House, Third Edition.

3. http://www.voip-info.org/wiki/view/ZRTP

4. https://en.wikipedia.org/wiki/H.323

5. Prateek Gupta, Vitaly Shmatikov http://www.cyber-ta.org/pubs/shmat_csf071.pdf

6. http://www.asterisk.org/

7. https://en.wikipedia.org/w/index.php?title=Business_telephone_system&redirect=no#Private_branch_exchange 

8. https://www1.pbxes.com/wiki/index.php/Getting_Started
