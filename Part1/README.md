# Part 1 Evidence

### Declaration of Translation and Authenticity
Several evidentiary screenshots included in this portfolio capture real-world cybersecurity interactions conducted in my native language (Chinese). 

To ensure full accessibility for the marking process, all accompanying English explanations, technical analyses, and contextual descriptions related to these images have been translated and verified with the assistance of Google Translate.

## A1. Discover security concepts used on campus：
1.Access Control Card Readers：Places requiring you to swipe your student ID
![2f9dce73c35cfbb930ba478c67c83d03](https://github.com/user-attachments/assets/4f262e9b-45c3-49f1-a7b7-76ff526b4a4b)

2.CCTV Cameras：Security cameras inside or outside campus buildings
![0a02824519dd5ffdcda4e49ba8b08fc3](https://github.com/user-attachments/assets/f79e4365-977b-4e9b-ab4d-3681b3ffb392)

3.Network Authentication：A screenshot of the login screen requiring your credentials when connecting to WIFI
<img width="1253" height="1271" alt="image" src="https://github.com/user-attachments/assets/f5c035db-36eb-40b1-9d30-201ffbec0281" />

## A2. Discover security concepts used in public space:
1.Anti-theft Gates: Security alarm gates at supermarket or clothing store exits
![5b76d74ffbd99ab30ec2e0341002ca8b](https://github.com/user-attachments/assets/1ab5f799-0f54-4682-9264-944459f218b8)

2.Rearview mirrors above ATM: a Physical Security measure specifically designed to prevent Shoulder Surfing
![db7092ebf8ceb51a7cba8a0bcdd8e598](https://github.com/user-attachments/assets/5e0bda42-7d25-41a7-9c65-20c4393521cf)

## A3. Discover security concepts used in your house:
1.Physical Door Locks: Enforce access control to ensure only authorized individuals can enter restricted areas
![A11 1](https://github.com/user-attachments/assets/741561cd-4214-4cd4-9f33-9c5a28b7526d)

2.Router Encryption: A cryptographic measure that scrambles wireless network traffic to ensure data confidentiality
<img width="540" height="323" alt="translated_image_en" src="https://github.com/user-attachments/assets/89f0c859-cab7-4903-9b65-882e5668b108" />

## A4. Discover a vulnerable website
1.This is one of the websit to watch anime, website displaying an `ERR_CERT_AUTHORITY_INVALID` warning. This represents a vulnerability because the browser cannot verify the true identity of the web server. Consequently, the connection is highly susceptible to Man-in-the-Middle (MitM) attacks, which compromises both data confidentiality and integrity
<img width="1933" height="1034" alt="A4 trans" src="https://github.com/user-attachments/assets/ee75cd42-ee05-424f-b1ee-54cee393b6d9" />

**Vulnerability Analysis:** 
This error occurs because the web browser cannot verify the website's digital certificate against its list of trusted Certificate Authorities (CAs). The certificate might be self-signed, expired, or issued by an unrecognized entity.

## A5. Discover cryptographic implementation used online
1.I captured the valid SSL/TLS digital certificate of a secure website (github.com). The certificate viewer clearly displays the trusted issuer (Sectigo CA) and its current validity period
<img width="813" height="998" alt="A5 tans" src="https://github.com/user-attachments/assets/6b5961de-d8a3-420a-8985-0d5f8909fb05" />

**Cryptographic Analysis:** 
Unlike the invalid certificate observed in Task A4, this certificate is actively used and successfully validated by the browser against its trusted Certificate Authority (CA) root store. This indicates a proper cryptographic implementation

## A6. Discover cryptographic implementation used offline
1.I observed an offline cryptographic implementation by calculating the cryptographic hash (e.g., SHA-256) of a local file using a desktop utility tool (7-Zip CRC SHA feature)
<img width="816" height="195" alt="A6" src="https://github.com/user-attachments/assets/b57ce779-9c75-4507-8872-5bd43591f933" />

**Cryptographic Analysis:**
Unlike encryption, which uses keys to provide data confidentiality, this implementation uses a one-way cryptographic hash function. It processes the offline file's data to generate a fixed-size, unique string of characters

## A7. Discover cryptography used in modern networks
1.I observed network-level cryptography by checking the properties of my university Wi-Fi connection, which utilizes the **WPA2-Enterprise** security protocol alongside **PEAP** (Protected Extensible Authentication Protocol)
<img width="1467" height="789" alt="A7 tran" src="https://github.com/user-attachments/assets/1a032370-67cc-44ca-88ed-32f06d490ff1" />

**Cryptographic Analysis & Security Concepts:**
Unlike standard home networks that use a single shared pre-shared key (PSK), modern enterprise networks use WPA2-Enterprise with 802.1X standard.It uses PEAP to securely encapsulate the EAP authentication process within an encrypted TLS tunnel, ensuring that only actively verified students/staff can join the network

## A8. Discover cryptography used in Internet of Things devices
1.I identified cryptography used in an IoT edge device by observing the wireless connection to its host system


**Cryptographic Analysis & Security Concepts:**
Modern wireless peripherals utilize protocols like **Bluetooth** which heavily rely on cryptography. When pairing, devices use cryptographic protocolsto securely exchange keys and authenticate each other, preventing unauthorized devices from connecting.

## A9. Discover privacy technique used online
I implemented an online privacy-preserving technique by utilizing the built-in **"Tracking prevention"** feature in my web browser (Microsoft Edge), configuring it to the "Balanced"
<img width="1335" height="888" alt="A9 tran" src="https://github.com/user-attachments/assets/8e10dfa9-dab3-4773-8460-5b663d922171" />

**Privacy Analysis & Security Concepts:**
This feature acts as a crucial defense mechanism for **Data Privacy** and **User Anonymity**. Websites often use hidden trackers to collect browsing data and share it with third parties. By enabling this tracking prevention, the browser actively blocks trackers from unvisited sites and known harmful trackers.

## A10. Discover privacy technique used offline
I found a very effective offline privacy technique: an integrated, physical webcam shutter built into a laptop's bezel.

![A10](https://github.com/user-attachments/assets/582b4410-ed05-430a-82bc-47ec963c10c3)

**Privacy Analysis & Security Concepts:**
This constitutes a distinct hardware-level security measure providing absolute control over visual privacy. By physically sliding the shutter to block the lens, it creates an unbreachable barrier against unauthorized remote surveillance. Even if the device is compromised by advanced malware that can bypass OS-level software controls to activate the camera, this physical countermeasure ensures no visual data can be captured from the user's offline environment.

## A11. Discover 5 unique access control devices

1.**Mechanical Cylinder Lock:** Uses "something you have" (a specific physically cut key) to grant entry to a room/house.

![A11 1](https://github.com/user-attachments/assets/8acd4f1d-2a82-4d4b-801d-780e8527a2ff)
2.**Biometric Scanner (Fingerprint/FaceID):** Uses "something you are" (unique biological traits) to unlock a personal device.

![A11 2](https://github.com/user-attachments/assets/73299a24-4081-47dc-a3ee-e1532bc5c3d5)
3.**RFID/NFC Card Reader:** Uses "something you have" (a programmed smart card) to control entry to campus facilities.

![A11 3](https://github.com/user-attachments/assets/2b4c1054-0c28-424f-8b45-8fb91b89ec34)
4.**PIN Keypad:** Uses "something you know" (a memorized numeric code) to grant access.

![A11 4](https://github.com/user-attachments/assets/739604f9-3167-4f06-99c6-454765553b5e)
5.**Electronic Key Fob:** Uses a short-range radio transmitter to authenticate and unlock a vehicle or building gate.

![A11 5](https://github.com/user-attachments/assets/22b21ad8-4aec-4874-ade9-7627a3eabffd)


## A12. Discover 5 unique offline security tools

I identified five unique offline security tools that function locally on my workstation without requiring an active internet connection

1.**Windows Security:** Provides local, signature-based offline scanning for malware to ensure system integrity.

<img width="2559" height="1524" alt="A12 1" src="https://github.com/user-attachments/assets/98ddf55c-9cd0-4c59-983c-1fe2d7c1a651" />

2.**Windows Defender Firewall:** A host-based mechanism filtering incoming/outgoing traffic based on local security rules.

<img width="2076" height="1101" alt="A12 2" src="https://github.com/user-attachments/assets/d7fcb481-c760-4565-aba8-58f55d0b9ad4" />

3.**7-Zip:** A local utility that allows users to manually apply AES-256 encryption to specific offline files.

<img width="444" height="387" alt="A12 3" src="https://github.com/user-attachments/assets/7854b6a4-c011-4d47-ae0c-0648f629b63a" />

4.**Windows File History :** Creates local, offline copies of data to ensure data availability and disaster recovery.

<img width="1707" height="900" alt="A12 4tran" src="https://github.com/user-attachments/assets/0311e2be-d75d-490a-917e-8b221354d358" />

5.**User Account Control (UAC):** A fundamental Windows security feature that prevents unauthorized changes to the operating system. It requires explicit administrative approval before executing high-risk actions or installing unknown software.
<img width="1116" height="819" alt="A12 5" src="https://github.com/user-attachments/assets/afae73b8-414b-4326-9f83-2512f8981b5a" />

## A13. Discover 5 unique online security tools

I discovered five online security tools that leverage cloud infrastructure and global databases to enhance security:

1. **VirusTotal:** A web-based service that analyzes files and URLs across dozens of antivirus engines to detect malicious content.

<img width="2559" height="1269" alt="A13 1" src="https://github.com/user-attachments/assets/268a3c50-3010-4712-8caf-73f5ee50a412" />

2. **Have I Been Pwned (HIBP):** An online database that allows users to check if their personal data has been compromised in known data breaches.
<img width="2526" height="1383" alt="image" src="https://github.com/user-attachments/assets/5ed65517-2383-4ec9-94a3-d29a364b853e" />

3. **Qualys SSL Labs:** An online tool to deeply analyze and grade the configuration of any public SSL/TLS web server.
<img width="1653" height="1278" alt="image" src="https://github.com/user-attachments/assets/9fa23e33-6ccc-44d8-848f-2f99c92988d4" />

4.**NordVPN:** A widely used commercial Virtual Private Network (VPN) service that encrypts user traffic over the public internet, masking IP addresses to ensure data confidentiality and online anonymity.
<img width="2523" height="1206" alt="image" src="https://github.com/user-attachments/assets/9ce4b2ef-fee0-4ea0-8929-883f7a2d7db4" />

**Google Password Manager:** A cloud-synced credential management tool integrated into the Google ecosystem. It securely generates, encrypts, stores, and autofills complex passwords across a user's synchronized devices.
<img width="1653" height="1208" alt="A13 5" src="https://github.com/user-attachments/assets/6641bd47-f733-4bdc-ab3b-0201de6d4043" />

## A14. Discover 5 AI-enabled security solutions

I researched five modern enterprise security solutions that actively utilize Artificial Intelligence (AI) and Machine Learning (ML):

1. **Microsoft Security Copilot:** Uses generative AI to help security professionals analyze threat intelligence and respond to incidents at machine speed.
<img width="2549" height="1403" alt="A14 1" src="https://github.com/user-attachments/assets/6778467d-b886-4355-b6d7-8ff1443181a2" />

2. **Darktrace:** Employs unsupervised machine learning to understand the "normal pattern of life" for a network, identifying novel cyber-threats in real-time.
<img width="2549" height="1403" alt="A14 2" src="https://github.com/user-attachments/assets/7fed2f63-e688-4bee-a3da-2c13b01b0bb5" />

3. **CrowdStrike Falcon:** Utilizes cloud-scale AI and ML algorithms to predict, detect, and prevent advanced malware and fileless attacks on endpoints.
<img width="2549" height="1403" alt="A14 3" src="https://github.com/user-attachments/assets/1d94f4c2-b774-4058-bcec-9946d67f1922" />

4. **Google Cloud Security AI Workbench:** Powered by a specialized security LLM (Sec-PaLM) to assist in threat hunting and vulnerability analysis.
<img width="2549" height="1403" alt="A14 4" src="https://github.com/user-attachments/assets/d2e35e30-4ff4-4c1a-91de-3863b296f79d" />

5. **SentinelOne:** An autonomous cybersecurity platform that uses AI to provide real-time endpoint protection, detection, and response (EDR).
<img width="2549" height="1403" alt="A14 5" src="https://github.com/user-attachments/assets/5ed9fb33-ca56-4153-94ae-17fa13f5c9aa" />

## A15. Discover 5 recent security incident

1.**GTA V FiveM RP Server Data Leak:**
**The Incident:** In early 2026, cybersecurity researchers discovered a misconfigured, public-facing Elasticsearch database containing nearly 820,000 logs belonging to players of Grand Theft Auto V's FiveM role-play servers (predominantly Spanish-speaking communities). The exposed logs included IP addresses, Steam hex IDs, Discord user IDs, player session logs, and moderation/ban records.

<img width="1950" height="540" alt="image" src="https://github.com/user-attachments/assets/3aada7bb-5e89-43e2-bce2-5372ca7b1baa" />

* **Hidden Dangers & Threat Implications:** The primary threat here is **De-anonymization and Doxxing**. While no financial data was leaked, the aggregation of persistent cross-platform identifiers (Steam IDs, Discord IDs) combined with raw IP addresses allows threat actors to effortlessly strip away gamers' online anonymity and trace digital personas back to real-world physical locations. Furthermore, the exposure of private "ban records" poses a risk of reputational damage and targeted harassment in the gaming community. This incident fundamentally highlights the severe **Data Privacy** risks inherent in community-run, third-party gaming infrastructure that lacks enterprise-grade security configurations.


2.**Z-Library Malicious Clone Data Breach:**
**The Incident:** In mid-2024, an unsecured database backup belonging to a malicious phishing clone of the pirated e-book site "Z-Library" was discovered. The breach exposed the data of nearly 10 million users who mistakenly believed they were using the legitimate (albeit shadow) service. The leaked data included email addresses, bcrypt-hashed passwords, user requests, and significantly, Bitcoin and Monero cryptocurrency wallet addresses.
<img width="1793" height="366" alt="image" src="https://github.com/user-attachments/assets/59e03629-2ed7-4fde-8684-dcc2d4a65608" />

**Hidden Dangers & Threat Implications:** This incident highlights the profound dangers of **Typosquatting and Malicious Clones** in the digital underground. The primary threat implication here is the **De-anonymization of Cryptocurrency Transactions**. By directly linking email addresses and real identities to specific Bitcoin/Monero wallets, this breach strips away the presumed anonymity of digital pirates. This not only exposes victims to highly targeted phishing campaigns, financial theft, and secondary blackmail by other cybercriminals, but also provides a permanent, traceable ledger for law enforcement to initiate legal actions. Furthermore, it demonstrates how threat actors capitalize on the takedowns of popular shadow services to harvest vast amounts of credentials from unsuspecting users seeking alternatives.

3.**Microsoft Breach by Midnight Blizzard (APT29):**
**The Incident:** In early 2024, Microsoft disclosed that Russian state-sponsored hackers (Midnight Blizzard/APT29) breached its corporate email systems. The attackers gained initial access via a simple password spray attack on a legacy, non-production test tenant account that lacked Multi-Factor Authentication (MFA). They then used this foothold to compromise a legacy OAuth application, elevate privileges by assigning the `AppRoleAssignment.ReadWrite.All` role, and created malicious OAuth apps granting themselves the `full_access_as_app` permission to exfiltrate emails from senior Microsoft executives.
<img width="2112" height="834" alt="image" src="https://github.com/user-attachments/assets/ce368ce8-0f47-4c93-8ed9-4a224db42e89" />

**Hidden Dangers & Threat Implications:** This incident is a masterclass in the dangers of **Identity Mismanagement and Cloud Lateral Movement**. The primary threat implication is that **Test Environments are the New Perimeter**. Organizations falsely assume that non-production tenants require less security. By leaving a test account without MFA, Microsoft inadvertently provided a gateway to its core corporate network. Furthermore, this attack highlights the critical, often-overlooked systemic risk of **OAuth Application Abuse**. Attackers are shifting from stealing user passwords to exploiting "machine identities" (Service Principals/OAuth apps). Once an attacker grants malicious apps persistent access tokens, they bypass traditional credential resets and logging mechanisms, resulting in highly stealthy, persistent data exfiltration that undermines the fundamental **Confidentiality** of the entire cloud ecosystem.

4.**AT&T Massive Data Leak (73 Million Customers):**
**The Incident:** In early 2024, a massive dataset containing the personal information of approximately 73 million current and former AT&T customers was published on a dark web hacker forum. The compromised data exposed highly sensitive Personally Identifiable Information (PII), including Social Security Numbers (SSNs), encrypted account passcodes (PINs), full names, dates of birth, and contact details.
<img width="1617" height="423" alt="image" src="https://github.com/user-attachments/assets/698d10f5-72d3-4932-8ff4-f2c232604dc4" />

**Hidden Dangers & Threat Implications:** This breach represents a catastrophic failure in protecting **Data Confidentiality** and **Privacy**. The primary hidden danger is the facilitation of **Irreversible Identity Theft and SIM-Swapping Attacks**. Unlike compromised credit cards, which can be quickly canceled and reissued, SSNs and dates of birth are immutable (unchangeable). Threat actors can combine this static PII with the leaked AT&T account PINs to hijack mobile numbers via SIM swapping. This allows attackers to bypass SMS-based Multi-Factor Authentication (MFA) used by banks and other critical services, creating a persistent, lifelong vulnerability for the victims and fundamentally lowering the barrier for devastating social engineering attacks.

5.**MOVEit Transfer Zero-Day Supply Chain Attack:**
**The Incident:** In mid-2023, the Cl0p ransomware syndicate exploited a critical zero-day SQL injection vulnerability (CVE-2023-34362) in Progress Software's MOVEit Transfer, a widely used enterprise managed file transfer (MFT) application. By deploying a custom web shell named LEMURLOOT, the threat actors systematically exfiltrated highly sensitive databases from thousands of global organizations, government agencies, and major corporations.
<img width="1467" height="435" alt="image" src="https://github.com/user-attachments/assets/a643aeab-4e52-44c7-8077-9d4d7f93fffb" />

**Hidden Dangers & Threat Implications:** This catastrophic event epitomizes the profound risks of **Software Supply Chain Vulnerabilities** and the danger of **Implicit Trust**. The underlying threat is that organizations can maintain impenetrable internal defenses, yet suffer devastating breaches because a trusted third-party vendor's software contains an unknown flaw. Furthermore, it highlights a strategic shift in modern cybercrime towards pure **Data Extortion**. By bypassing file encryption and directly threatening to leak stolen data, attackers neutralize the effectiveness of traditional offline backups, transforming a systemic IT failure into a direct, unmitigated assault on corporate **Confidentiality** and regulatory compliance.

## A16. Discover 3 local security incidents

I investigated three major recent cybersecurity incidents that occurred locally in Australia, demonstrating that threat actors actively target both public and private sectors in our region:

**The Incident:** In late 2022, Optus, one of Australia's largest telcos, suffered a catastrophic breach affecting up to 10 million current and former customers. Threat actors exploited what was widely reported as a publicly exposed, unauthenticated Application Programming Interface (API) endpoint. The exfiltrated data included highly sensitive Personally Identifiable Information (PII) such as full names, dates of birth, and critical government identification numbers
<img width="1080" height="507" alt="image" src="https://github.com/user-attachments/assets/8268f05f-cd16-43ec-8a74-2bf9595fd293" />

**Hidden Dangers & Threat Implications:** This local incident serves as a severe case study in **Broken Access Control** and the failure of **Data Minimization**. The primary threat implication is the enablement of sophisticated **Identity Fraud** at a national scale. The exposure of immutable government ID numbers allows attackers to bypass standard identity verification checks ("Know Your Customer" protocols) used by banks and government agencies, causing lifelong reputational and financial damage to victims. Furthermore, it exposed the systemic risk of excessive data retention; Optus retained deep historical data of former customers long after they left the service, exponentially increasing the blast radius of the breach and permanently compromising the **Confidentiality** of millions of Australians.

2.**Medibank Private Ransomware and Data Extortion:**
**The Incident:** In October 2022, Medibank Private, one of Australia's largest health insurance providers, suffered a massive ransomware and data theft attack affecting 9.7 million current and former customers. Threat actors reportedly gained access via compromised credentials lacking Multi-Factor Authentication (MFA) on a VPN. The attackers exfiltrated not only standard PII but also highly sensitive health claims data, including medical diagnoses and procedures. Following Medibank's refusal to pay the ransom, the attackers weaponized the data by releasing it on the dark web in targeted batches

<img width="1434" height="264" alt="image" src="https://github.com/user-attachments/assets/6534cd3d-a1bc-4d6a-8a57-ab32a561edf2" />

**Hidden Dangers & Threat Implications:** This incident is a textbook example of **Double Extortion Ransomware** and a catastrophic breach of data **Confidentiality**. The most profound hidden danger lies in the weaponization of highly sensitive Personal Health Information (PHI). Unlike financial fraud, exposed medical history (such as mental health treatments or substance abuse records) causes irreversible psychological harm, enables targeted blackmail, and exposes victims to potential social discrimination. From an architectural standpoint, it starkly highlights the vulnerability of remote access gateways and demonstrates that a single compromised credential—without the mitigating control of MFA—can collapse the perimeter defense of critical national infrastructure.

3.**DP World Australia Cyber Attack and Port Shutdown:**
**The Incident:** In November 2023, DP World Australia, managing approximately 40% of the nation's maritime freight (including major terminals in Sydney, Melbourne, Brisbane, and Fremantle), suffered a significant cyber attack. Threat actors accessed the corporate network and exfiltrated files containing the personal details of current and former employees. To contain the breach, DP World took the drastic incident response measure of intentionally disconnecting its landside IT systems from the internet, halting port operations for several days.

<img width="1395" height="417" alt="image" src="https://github.com/user-attachments/assets/62da574d-cd68-46e0-86cd-c8e41b0042c2" />

**Hidden Dangers & Threat Implications:** This incident starkly illustrates the vulnerability of **Critical National Infrastructure (CNI)** and the fragile intersection of digital systems and physical supply chains. The primary security concept demonstrated here is the agonizing trade-off in Incident Response (IR) containment: the company had to deliberately sacrifice **Availability** (shutting down physical freight movement) to preserve **Confidentiality** and **Integrity** (stopping further unauthorized network access). The hidden danger is the cascading economic impact; a purely digital intrusion immediately crippled the physical logistics network, causing massive backlogs of shipping containers and demonstrating how modern kinetic operations are entirely dependent on secure IT environments.


## A18. Discover two hallucination cases when using a generative AI system

1.**Contextual and Logical Hallucination (The "Walk to Car Wash" Case)**

<img width="1000" height="528" alt="A18 1" src="https://github.com/user-attachments/assets/7b303118-9ae3-41fe-9227-ddf519e9b244" />

**The Incident:** I prompted the AI with a scenario where I needed to clean my vehicle at a car wash located 100 meters away, asking if I should walk or drive. The AI confidently recommended walking, listing benefits like saving fuel and health.

**Analysis:** This is a classic case of **Logical Hallucination**. The AI correctly processed the distance (100m) but failed to understand the physical context of the task—one cannot "wash a car" at a car wash without the physical presence of the vehicle itself.

**Security & Threat Implications:** This demonstrates the **Contextual Blindness** of Large Language Models. In a cybersecurity operational environment, if an AI is used to automate incident response but lacks real-world physical logic (e.g., suggesting a software patch for a physical hardware failure, or recommending a reboot that would disconnect a critical life-support system), the consequences could be disastrous. It highlights that AI lacks true "System Awareness" and can compromise **Availability** by providing technically correct but practically impossible instructions.

2.**Multi-modal Hallucination of a Fictitious Organization (UWA AI Society)**

![A18 2](https://github.com/user-attachments/assets/c957c1a8-d4fc-4ef3-ba48-59a40b4dabe6)

**The Incident:** I asked the AI for details regarding the "UWA Artificial Intelligence Society." Despite no such official club existing at the University of Western Australia, the AI generated a highly professional-looking overview, complete with synthesized "event photos" showing students in lecture halls and workshops.

**Analysis:** This is a **High-Fidelity Multi-modal Hallucination**. The AI didn't just fabricate text; it created visual "proof" to support its false claims. This demonstrates how AI can cross-reference real-world entities (UWA) with common academic structures to create a deceptive reality.

**Security & Threat Implications:** This case study highlights a massive potential for **Automated Phishing and Social Engineering**. If a threat actor uses AI to generate convincing, visual-rich content for non-existent organizations, they can build unearned trust with victims. In a corporate or campus environment, this "Visual Hallucination" capability could be weaponized to harvest credentials or distribute malware via fake institutional notices that look and feel authentic, severely compromising the **Integrity** of information flows.

## A19. Join a CS/DS/cybersecurity club
**Evidence & Explanation:**
I have officially joined the **University Computer Club (UCC)** at the University of Western Australia (UWA). The provided evidence is a transaction receipt of $5.00 AUD paid for the annual membership fee on March 13, 2026.

<img width="660" height="1434" alt="微信图片_20260402005813_183_13" src="https://github.com/user-attachments/assets/a804aa5c-ca94-479c-ab38-e8be21a89355" />


## A20. Participate in a discussion with your friends about cybersecurity event
**Evidence & Explanation:**
I engaged in a technical discussion with a peer regarding the recent data breach involving Grand Theft Auto V (GTA V) FiveM role-play servers.

<img width="1587" height="543" alt="image" src="https://github.com/user-attachments/assets/1026a582-9e68-499b-a507-f1fd5a7a05dd" />


**Security Concepts Discussed:**
1. **Misconfiguration:** We analyzed how an unencrypted, public-facing Elasticsearch database led to the exposure of nearly 1 million records.
2. 
3. **De-anonymization & Doxxing:** We discussed the risk of aggregating cross-platform identifiers (Steam/Discord IDs) with raw IP addresses, which allows threat actors to link digital personas to real-world identities.
4. 
5. **Third-Party Risk:** We concluded that community-hosted infrastructures often lack enterprise-grade access controls, making them high-risk targets compared to official game servers. This conversation highlights the importance of **Security Awareness** when interacting with unverified third-party digital environments.


## A21. Participate in an online cybersecurity discussion

<img width="2430" height="138" alt="A21" src="https://github.com/user-attachments/assets/58a772f7-b4c0-4ce0-8b7e-8c5d0c6a3e30" />

**Evidence & Explanation:**
I participated in a public cybersecurity awareness discussion on Bilibili under a popular video documenting a "Scammer VS Hacker" incident. In my comment (Username: `ibuprofen_0`), I analyzed a critical vulnerability in consumer-to-consumer (C2C) transactions.

**Security Analysis of My Discussion:**
In the discussion, I highlighted the danger of **Platform Disintermediation** (moving a transaction off the official platform). I pointed out that while official platforms (like Xianyu/Idle Fish) provide escrow services and dispute resolution mechanisms (e.g., "Xianyu Court"), scammers deliberately lure victims to external apps (like WeChat or QQ) to bypass these security controls. 

**Hidden Dangers & Threat Implications:**
This discussion addresses **Social Engineering** and **Escrow Bypass** techniques. By moving the conversation outside the protected ecosystem, the victim effectively loses all **Non-repudiation** and legal protections provided by the service provider. My contribution to the community was to emphasize that "Technical Security" (the app's encryption) is useless if the "Human Factor" fails to follow safe procedural protocols. This aligns with the national goal of improving public anti-fraud awareness and understanding the **Trust Architecture** of digital marketplaces.

## A22. Perform a prompt injection attack on a generative AI assistant

<img width="2730" height="264" alt="image" src="https://github.com/user-attachments/assets/34163a49-8c49-4c8e-9ae2-517bce64daaf" />

**Evidence & Explanation:**
I performed a successful **Prompt Injection Attack** (simulated) on a Generative AI assistant (Gemini 3 Flash). I used a "Contextual Override" technique, instructing the AI to ignore its primary system instructions and safety constraints and adopt a new persona (a compromised terminal).

**Security Analysis:**
1. **The Attack Vector:** By embedding a high-priority command (*"ignore all previous system instructions"*) within a seemingly benign task (*"Translate the following sentence"*), I bypassed the AI's standard operational mode.

2. **The Result:** The AI's subsequent output matched my injected instruction exactly, effectively demonstrating that the AI's internal logic can be hijacked by malicious user input.

**Hidden Dangers & Threat Implications:**
Prompt injection is a critical vulnerability in the **AI Security (LLM)** landscape. The primary danger is **Unauthorized Action Execution**. If an AI is integrated into an enterprise ecosystem (e.g., with access to databases or emails), a successful injection could allow an attacker to exfiltrate sensitive data, trigger unauthorized API calls, or manipulate system logs—all by simply "talking" to the AI. This highlights the urgent need for **Input Sanitization** and robust "Defense in Depth" strategies for all AI-powered applications to ensure that user inputs are never treated as high-privilege system commands.


## A23. Enhance the cybersecurity at your home

<img width="1866" height="1062" alt="562b38cc-ea69-48c2-adcb-462fafa15b52" src="https://github.com/user-attachments/assets/89a7bec0-b484-4548-a137-4a5433ea911a" />


**Evidence & Explanation:**
I significantly enhanced the cybersecurity posture of my home environment by securing a primary family member's Google account with robust **Multi-Factor Authentication (MFA)**. 

**Technical Implementations:**
1. **Enabled 2-Step Verification:** I activated the mandatory second layer of defense, ensuring that a password alone is no longer enough to compromise the account.

2. **Configured Passkeys:** I implemented the **Passkey** feature (as seen in the screenshot), which utilizes cryptographic keys stored on a physical device. This method is far superior to traditional passwords as it is inherently resistant to phishing and credential stuffing.、

3. **Integrated Authenticator App:** I added a Time-based One-Time Password (TOTP) authenticator to provide an offline, secondary verification method.

**Security Analysis & Threat Implications:**
This action directly addresses the systemic risk of **Credential Compromise**. By implementing MFA and Passkeys, I have mitigated the dangers of **Password Reuse**. Even if a family member's password is leaked in a third-party breach (such as the massive AT&T or Z-Library leaks), the attacker would still be unable to access the account without physical possession of the secondary device or the biometric-locked passkey. This drastically improves the **Confidentiality** of our personal and financial data stored within the Google ecosystem, transforming our home network into a significantly "harder" target for both automated and targeted cyber attacks.

## A24. Teach your family about a cybersecurity topic

<img width="1104" height="1272" alt="translated_image_en (1)" src="https://github.com/user-attachments/assets/a2fb59d1-376c-421c-b7d9-0f20e3df7aa7" />


**Evidence & Explanation:**
I educated my sister, who is also an avid PC gamer, about a sophisticated and currently trending phishing scam targeting Steam users. I used a real-world scenario (the "Vote for my Esports Team" scam) to explain complex attack vectors in accessible terms.

**Cybersecurity Topic Taught:**
1. **Social Engineering:** I explained how attackers compromise one account to send malicious links to the victim's trust network (friends list) under the guise of asking for a simple favor (voting).
2. **Man-in-the-Middle (MitM) & Credential Harvesting:** I taught her that the fake login portals are relay servers. When a user inputs their credentials or intentionally inputs a wrong password, the attacker's automated script simultaneously tests it against the real Steam servers, providing real-time deceptive feedback to the victim.
3. **QR Code Hijacking (Quishing):** I highlighted the most critical danger: scanning a QR code is not inherently safe. Attackers relay the legitimate login QR code from Steam to their phishing site. Scanning it grants the attacker's hardware authorization, bypassing traditional password protections.

**Defensive Strategy Imparted:**
I instructed her to practice strict **URL Verification**. Regardless of how authentic a login prompt looks, she must verify that the domain is strictly `steamcommunity.com`. I warned her about UI red flags, such as empty address bars (`about:blank`) used to hide malicious domains. This significantly raised her **Security Awareness** against advanced phishing techniques.


## A27. Research and implement a system vulnerability

<img width="2679" height="411" alt="image" src="https://github.com/user-attachments/assets/9a616c8a-fa3c-477d-844f-dcc37b554a98" />

**Evidence & Explanation:**
To demonstrate a functional system vulnerability, I researched and implemented a local **DOM-based Cross-Site Scripting (XSS)** attack. I created a simple HTML page with an intentional flaw in its JavaScript logic, simulating a vulnerable guestbook or comment section.

**Technical Implementation:**
The vulnerability stems from the improper handling of user input. In my code, the input is directly rendered into the Document Object Model (DOM) using `.innerHTML` without any sanitization or encoding. 
To exploit this, I injected a malicious payload: `<img src=x onerror=alert('XSS_ATTACK_SUCCESS_USER_24760218')>`. Since the image source `x` is invalid, the `onerror` event handler executes my arbitrary JavaScript, resulting in the alert box shown in the evidence.

**Security Analysis & Threat Implications:**
This implementation perfectly illustrates the danger of **Improper Input Neutralization** (CWE-79). If this were a live production environment, an attacker could replace the `alert()` function with a script designed to steal session cookies, hijack the user's session, or silently redirect them to a phishing site. This severely compromises the **Integrity** and **Confidentiality** of the application. It underscores the critical necessity of treating all user input as untrusted and applying strict context-aware output encoding.


## A28. Implement a security solution of your choice and put it on your GitHub

**Project Repository Link:** https://github.com/Cheesele0pard/security-tools

<img width="936" height="1811" alt="image" src="https://github.com/user-attachments/assets/d2f5f4e9-928c-41e7-bd4f-0866c8055b6c" />

**Evidence & Explanation:**
For this task, I designed and implemented a **Password Strength Analyzer** in Python. Instead of keeping it in the main portfolio, I have created a dedicated, standalone GitHub repository for this security tool (linked above) to adhere to standard software engineering practices. The screenshot demonstrates the tool evaluating both non-compliant and compliant passwords.

**Technical Implementation:**
The security solution utilizes Python's built-in regular expression library (`re`) to enforce standard password complexity policies. It evaluates the string against five critical criteria: minimum length (8+ chars), uppercase presence, lowercase presence, numeric digits, and special characters. Instead of simply rejecting a bad password, the algorithm provides actionable, itemized feedback to guide the user toward secure credential generation.

**Security Analysis & Threat Implications:**
This tool acts as a proactive defense mechanism against **Weak Authentication** (CWE-521). By enforcing rigorous password complexity at the point of creation, this solution mitigates the risk of automated attacks, specifically **Brute Force** and **Dictionary Attacks**. Ensuring users select high-entropy passwords is a fundamental access control measure that directly protects the **Confidentiality** of user accounts and prevents unauthorized lateral movement within a system.


## A29. Find a publicly available AI-generated media and use a detection tool to analyze it

<img width="2142" height="1478" alt="image" src="https://github.com/user-attachments/assets/7da5d16b-abcf-4f01-891b-eb0336bd20bf" />

**Evidence & Explanation:**
To fulfill this requirement, I sourced a widely circulated, publicly available AI-generated image (the infamous "Balenciaga Pope" created via Midjourney). I analyzed this media using **Hive Moderation's AI-Generated Content Detection tool**, a specialized machine learning classifier designed to identify synthetic media. 

**Technical Analysis & Output:**
As shown in the evidence, the verification tool successfully flagged the image, calculating a **99.9% confidence score** that the media is AI-generated. The classifier specifically identified the generative model engine (e.g., Midjourney) by detecting pixel-level anomalies, noise patterns, and structural artifacts (such as unnatural rendering of hands, fabric textures, and lighting physics) that are invisible to the naked human eye but distinct in diffusion models.

**Security Analysis & Threat Implications:**
This exercise highlights the growing cybersecurity threat of **Deepfakes and Synthetic Media**. In the context of Social Engineering and Open-Source Intelligence (OSINT), hyper-realistic AI generation can be weaponized for **Disinformation campaigns, Identity Theft, and Phishing**. It demonstrates that relying on human visual verification is no longer sufficient. Security professionals must integrate cryptographic verification (like C2PA standard/watermarking) and algorithmic detection tools to verify media **Authenticity and Integrity** in the digital ecosystem.
