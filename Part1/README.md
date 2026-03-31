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

