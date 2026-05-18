# Part 1 Evidence

## B1. Discover 5 unique weak/vulnerable security implementations.


<img width="1656" height="672" alt="B1（1）" src="https://github.com/user-attachments/assets/e9be494b-db35-4c6b-b8c5-56ec2aa9cc72" />
the login page for the TP-Link router's management console (hosted at the local IP address 192.168.1.1) is accessed via the unencrypted HTTP protocol. The web browser explicitly flags the connection as "Not secure"

<img width="1872" height="537" alt="B1(2)" src="https://github.com/user-attachments/assets/61a30ebe-55f7-4fa5-8d52-039f5960a77b" />
The authentication interface returning a specific error message indicating the non-existence of an account.The system explicitly confirms whether a specific user exists in its database.This verified list can then be leveraged to launch targeted Brute Force attacks

<img width="1581" height="945" alt="B1(3)" src="https://github.com/user-attachments/assets/555bb229-f07c-4b77-82bf-16f3ee4e1f87" />
The registration form allowing the creation of an account with a highly common password ("abc1234"), despite displaying a frontend warning about its weakness.

<img width="1878" height="489" alt="B1(4)" src="https://github.com/user-attachments/assets/3db375c4-d742-4812-bbe5-77d685d81983" />
As demonstrated in the screenshot, the authentication system permits repeated, consecutive login attempts with incorrect passwords without triggering any defensive mechanisms.

## B2. Discover 5 unique strong security implementations.


<img width="900" height="1176" alt="B2(1)" src="https://github.com/user-attachments/assets/4f1701b0-029e-4532-ad89-d2fe97f22a0c" />
Nintendo Account login interface prompting the user to authenticate using a biometric passkey.the system allows the user to log in using device-bound biometric verification。

<img width="1320" height="595" alt="B2(2)" src="https://github.com/user-attachments/assets/f14cc32a-5b13-44ab-848e-3cebd2f0ebd3" />
Messaging application displaying an end-to-end encryption notification. The system ensures that data is encrypted on the sender's device and can only be decrypted by the intended recipient, preventing third-party interception.

<img width="627" height="366" alt="B2(3)" src="https://github.com/user-attachments/assets/4e6bbe87-8c2b-4b78-b3fd-55d0db4a29c1" />
Login interface integrating an invisible CAPTCHA (Cloudflare Turnstile). This system silently verifies human behavior in the background to block automated bot attacks and brute-force login attempts.

<img width="666" height="1080" alt="B2(4)" src="https://github.com/user-attachments/assets/b20c0d6f-286b-462a-a3d9-a147b832bcbc" />
Registration interface enforcing a strict password length policy. The system rejects short, weak passwords and explicitly requires a minimum of 8 characters to prevent brute-force and dictionary attacks.

<img width="1320" height="517" alt="B2(5)" src="https://github.com/user-attachments/assets/cf8da771-a713-4e8e-9ca7-b42d9047d23a" />
the system enforces Multi-Factor Authentication (MFA) utilizing the Microsoft Authenticator app. When attempting to access the account from a new or unrecognized device

## B3. Discover 3 proactive security implementations in practice

<img width="738" height="645" alt="B3(1)" src="https://github.com/user-attachments/assets/d1e5bb41-23e4-4fa5-b397-a45cabccd5bb" />
Microsoft Defender actively intercepting the EICAR test string immediately upon file creation.a text document containing the EICAR standard anti-virus test signature was created on the desktop. Immediately upon pasting the string and saving the file, Microsoft Defender's real-time protection module proactively scanned the file's contents.

<img width="1590" height="1256" alt="B3(2)" src="https://github.com/user-attachments/assets/c1bde5aa-ef00-493f-9361-fd53b505b454" />
A Cloudflare WAF block page proactively intercepting a potentially malicious HTTP request.When a request containing potentially malicious payloads (such as test SQL commands or illegal keywords) was submitted, the system's Web Application Firewall (WAF) intercepted the traffic.

<img width="1572" height="987" alt="B3(3)" src="https://github.com/user-attachments/assets/d7709aa6-3ff6-4e3d-ba59-740ccef7484c" />
Google Chrome displaying a full-screen red warning, proactively blocking navigation to a known phishing URL based on Threat Intelligence.Before the webpage could load or execute any scripts, the browser displayed a prominent red warning screen. It explicitly halted the navigation process and urged the user to return to safety.

## B4. Participate in 3 in-class activities in labs (facilitators will administer such activities).

<img width="1279" height="2275" alt="B4(1)" src="https://github.com/user-attachments/assets/493f3ff8-faa2-434b-90e1-70c632f70cbd" />
Lab8
<img width="1279" height="2275" alt="B4(2)" src="https://github.com/user-attachments/assets/80e72163-9f73-4648-ad56-43f6cc4e5faf" />
Lab3
<img width="1320" height="1747" alt="B4(3)" src="https://github.com/user-attachments/assets/1aecf579-f4eb-4bfc-bbf9-d222f43d9b41" />
Lab1

## B9. Participate in an industry-related cybersecurity event.

<img width="4032" height="2268" alt="B9" src="https://github.com/user-attachments/assets/be6bd2a4-1484-418b-a0c3-c62875eda096" />
Lecture Title:Fraud Detection in the Real World — From Cybersecurity to the Banking Sector
