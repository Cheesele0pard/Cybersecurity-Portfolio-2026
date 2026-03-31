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
<img width="1947" height="1041" alt="ScreenShot_2026-03-08_203854_906" src="https://github.com/user-attachments/assets/7d942840-8cd9-4d26-b336-389d308563d5" />

**Vulnerability Analysis:** 
This error occurs because the web browser cannot verify the website's digital certificate against its list of trusted Certificate Authorities (CAs). The certificate might be self-signed, expired, or issued by an unrecognized entity.

## A5. Discover cryptographic implementation used online
1.I captured the valid SSL/TLS digital certificate of a secure website (github.com). The certificate viewer clearly displays the trusted issuer (Sectigo CA) and its current validity period
<img width="813" height="998" alt="A5" src="https://github.com/user-attachments/assets/ca637862-e4a1-44cb-9121-a163792e81fe" />

**Cryptographic Analysis:** 
Unlike the invalid certificate observed in Task A4, this certificate is actively used and successfully validated by the browser against its trusted Certificate Authority (CA) root store. This indicates a proper cryptographic implementation

## A6. Discover cryptographic implementation used offline
1.I observed an offline cryptographic implementation by calculating the cryptographic hash (e.g., SHA-256) of a local file using a desktop utility tool (7-Zip CRC SHA feature)
<img width="816" height="195" alt="A6" src="https://github.com/user-attachments/assets/b57ce779-9c75-4507-8872-5bd43591f933" />

**Cryptographic Analysis:**
Unlike encryption, which uses keys to provide data confidentiality, this implementation uses a one-way cryptographic hash function. It processes the offline file's data to generate a fixed-size, unique string of characters

## A7. Discover cryptography used in modern networks
1.I observed network-level cryptography by checking the properties of my university Wi-Fi connection, which utilizes the **WPA2-Enterprise** security protocol alongside **PEAP** (Protected Extensible Authentication Protocol)
<img width="1467" height="789" alt="A7" src="https://github.com/user-attachments/assets/b584f061-77bd-44a5-967e-6454e3bdb091" />

**Cryptographic Analysis & Security Concepts:**
Unlike standard home networks that use a single shared pre-shared key (PSK), modern enterprise networks use WPA2-Enterprise with 802.1X standard.It uses PEAP to securely encapsulate the EAP authentication process within an encrypted TLS tunnel, ensuring that only actively verified students/staff can join the network

## A8. Discover cryptography used in Internet of Things devices
1.I identified cryptography used in an IoT edge device by observing the wireless connection to its host system


**Cryptographic Analysis & Security Concepts:**
Modern wireless peripherals utilize protocols like **Bluetooth** which heavily rely on cryptography. When pairing, devices use cryptographic protocolsto securely exchange keys and authenticate each other, preventing unauthorized devices from connecting.

## A9. Discover privacy technique used online
I implemented an online privacy-preserving technique by utilizing the built-in **"Tracking prevention"** feature in my web browser (Microsoft Edge), configuring it to the "Balanced"
<img width="1335" height="888" alt="A9" src="https://github.com/user-attachments/assets/94f136ab-96b2-4896-a712-edc88acfb229" />

**Privacy Analysis & Security Concepts:**
This feature acts as a crucial defense mechanism for **Data Privacy** and **User Anonymity**. Websites often use hidden trackers to collect browsing data and share it with third parties. By enabling this tracking prevention, the browser actively blocks trackers from unvisited sites and known harmful trackers.

## A10. Discover privacy technique used offline
I found a very effective offline privacy technique: an integrated, physical webcam shutter built into a laptop's bezel.

![A10](https://github.com/user-attachments/assets/582b4410-ed05-430a-82bc-47ec963c10c3)

**Privacy Analysis & Security Concepts:**
This constitutes a distinct hardware-level security measure providing absolute control over visual privacy. By physically sliding the shutter to block the lens, it creates an unbreachable barrier against unauthorized remote surveillance. Even if the device is compromised by advanced malware that can bypass OS-level software controls to activate the camera, this physical countermeasure ensures no visual data can be captured from the user's offline environment.

