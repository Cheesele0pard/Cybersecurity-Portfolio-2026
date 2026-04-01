# Part 1 Evidence

## A1. Discover security concepts used on campus：
1.Access Control Card Readers：Places requiring you to swipe your student ID

2.CCTV Cameras：Security cameras inside or outside campus buildings

3.Network Authentication：A screenshot of the login screen requiring your credentials when connecting to WIFI

## A2. Discover security concepts used in public space:
1.Anti-theft Gates: Security alarm gates at supermarket or clothing store exits

2.Rearview mirrors above ATM: a Physical Security measure specifically designed to prevent Shoulder Surfing

## A3. Discover security concepts used in your house:
1.Physical Door Locks: Enforce access control to ensure only authorized individuals can enter restricted areas

2.Router Encryption: A cryptographic measure that scrambles wireless network traffic to ensure data confidentiality

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

2. **Medibank Private Ransomware and Data Extortion:**
**The Incident:** In October 2022, Medibank Private, one of Australia's largest health insurance providers, suffered a massive ransomware and data theft attack affecting 9.7 million current and former customers. Threat actors reportedly gained access via compromised credentials lacking Multi-Factor Authentication (MFA) on a VPN. The attackers exfiltrated not only standard PII but also highly sensitive health claims data, including medical diagnoses and procedures. Following Medibank's refusal to pay the ransom, the attackers weaponized the data by releasing it on the dark web in targeted batches
<img width="1434" height="264" alt="image" src="https://github.com/user-attachments/assets/6534cd3d-a1bc-4d6a-8a57-ab32a561edf2" />

**Hidden Dangers & Threat Implications:** This incident is a textbook example of **Double Extortion Ransomware** and a catastrophic breach of data **Confidentiality**. The most profound hidden danger lies in the weaponization of highly sensitive Personal Health Information (PHI). Unlike financial fraud, exposed medical history (such as mental health treatments or substance abuse records) causes irreversible psychological harm, enables targeted blackmail, and exposes victims to potential social discrimination. From an architectural standpoint, it starkly highlights the vulnerability of remote access gateways and demonstrates that a single compromised credential—without the mitigating control of MFA—can collapse the perimeter defense of critical national infrastructure.

3. **DP World Australia Cyber Attack and Port Shutdown:**
**The Incident:** In November 2023, DP World Australia, managing approximately 40% of the nation's maritime freight (including major terminals in Sydney, Melbourne, Brisbane, and Fremantle), suffered a significant cyber attack. Threat actors accessed the corporate network and exfiltrated files containing the personal details of current and former employees. To contain the breach, DP World took the drastic incident response measure of intentionally disconnecting its landside IT systems from the internet, halting port operations for several days.
<img width="1395" height="417" alt="image" src="https://github.com/user-attachments/assets/62da574d-cd68-46e0-86cd-c8e41b0042c2" />

**Hidden Dangers & Threat Implications:** This incident starkly illustrates the vulnerability of **Critical National Infrastructure (CNI)** and the fragile intersection of digital systems and physical supply chains. The primary security concept demonstrated here is the agonizing trade-off in Incident Response (IR) containment: the company had to deliberately sacrifice **Availability** (shutting down physical freight movement) to preserve **Confidentiality** and **Integrity** (stopping further unauthorized network access). The hidden danger is the cascading economic impact; a purely digital intrusion immediately crippled the physical logistics network, causing massive backlogs of shipping containers and demonstrating how modern kinetic operations are entirely dependent on secure IT environments.

     
