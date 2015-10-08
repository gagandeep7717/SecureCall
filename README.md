# SecureCall
Peer to peer voice communication using ZRTP

Project Members: 	Gagandeep Singh Randhawa and Aniket Nade

####Problem Statement
VoIP Strategy has been around for a while, using the data connectivity to transmit and receive voice. VoIP is made practical on mobiles by the data speed offered by mobile networks recently. But security in VoIP remains of top concern as voice packets are delivered over public internet, Also the confidentiality is at risk as it uses transparent IP protocol suite. Using Cryptographic key exchange to encrypt media stream is quite difficult task. Voice communications over VoIP are vulnerable to man in the middle attack. There is a need of stronger mechanism that protects voice packets from such vulnerabilities.

####Proposed solution
We propose to make use of Pretty Good Privacy (PGP) as strong cryptography protocol for voice communication. PGP is a scheme that provides data encryption and decryption with cryptographic privacy and authentication. It is often used for encrypting and decrypting e-mails, files and texts. This will prevent the adversary from intercepting the communication being held over the internet. We aim to establish an end to end connection between two parties. We are planning to involve android smartphones as the end points. VoIP simulation will be done via Asterisk (An Open Source VoIP simulator)
Following are the protocols to be used in implementation:

**ZRTP**: Zimmerman, Real-time Transport Protocol (ZRTP) is a cryptographic key-agreement protocol to negotiate the keys for encryption between two end points in a Voice over Internet Protocol (VoIP) phone telephony call based on the Real-time Transport Protocol. It uses Diffie–Hellman key exchange and the Secure Real-time Transport Protocol (SRTP) for encryption.

**SIP**: The Session Initiation Protocol (SIP) is a communications protocol for signaling and controlling multimedia communication sessions. SIP is commonly used in Internet telephony for voice and video calls, as well as instant messaging all over Internet Protocol (IP) networks.

**H323**: H323 is a protocol Standardized by the International Telecommunication Union (ITU), H323 is a signaling approach used for the deployment of VoIP systems. This protocol defines call setup messages and procedures used to establish a call, as well as messages and procedures used for user’s registration. It also defines security profiles such as authentication, message integrity, signature security, and voice encryption.

####Details of implementation
**Platform**: Android

**Programming Language**: Java

**Components Involved**: 
-	VoIP simulation tool (Asterisk)
-	Wireshark
-	PGP libraries provided by OpenPGP

####Timeline of Work
-	**14th September - 27th September**
  -	Understanding Mobile VoIP implementation
  -	Potential vulnerabilities in VoIP systems
- **28th September - 20th October**
  - Understanding Pretty Good Privacy protocol
  - Study implementation of PGP in java
  - Studying key exchange mechanisms
-	**21st October - 20th November**
  -	Integrating PGP into VoIP
  -	VoIP simulation using Asterisk
  -	Performance analysis of the system.


