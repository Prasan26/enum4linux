---
description: >-
  Understand the methodology followed by the hackers to attack a web server and
  discuss necessary countermeasures against Web server attacks.
---

# WEEK 7

Online Services became one of the significant factors for every Company's services. The ability to provide online services for public use would increase company business, value, and productivity. Different web applications became a daily habit of interacting and getting used to it, whether social, entertainment, or even eCommerce. However, nothing is for free. Attackers are continuously trying to break into company web services for different causes; political, financial gain, or competitive.

Due to the Privacy shield act, organizations are responsible for protecting user data and seeking accountability for such exploits that can expose users' data. It is no more concerned with securing company confidential data, but it also encompasses users' PII information used chiefly within our modern web application. Due Care expresses the Company's effort to protect, prevent attacks and reduce the risk associated with threat to an acceptable level.

First, we may need to understand the methodologies used for web server attacks before going through applicable countermeasures to implement.

Following are the stages of web server's attack methodology:

1. **Information Gathering**

Attackers aim to collect and gather as much information as possible about the target service. Once the attacker has obtained this information, he would analyze and figure out applicable loopholes within current security countermeasures. Following are standard tools to perform such action

* Whois \(https://whois.domaintools.com/\)
* Netcraft \([https://netcraft.com \(Links to an external site.\)](https://netcraft.com/)\)
* Robotext \([https://www.robtex.com/ \(Links to an external site.\)](https://www.robtex.com/)\)
* Search Engines \(google, Bing, Yahoo, etc.\)
* Social/Professional Networking \(Facebook, Twitter, LinkedIn, etc.\)

1. **Web Server Footprinting**

In this stage, the attacker undertakes possible tools to understand and discover more about web services capabilities, OS, ports, and services. The attacker uses footprinting and enumeration tools as following

* NMAP \(nmap -O -A -Pn -T4 -p80,443 TARGET\_IP
* View Page Source checking
* Search for Well Known Files as Robots.txt
* Recon-ng _\(_[_https://bitbucket.org \(Links to an external site.\)_](https://bitbucket.org/)_\)_

1. **Website Mirroring**

IT is commonly used to take an offline copy of a website and its content. In such a way , an attacker can view the detailed structure of the website.

* WebCopier Pro.
* Website Ripper Copier.
* GNU Wget.
* Pavuk Web Spider and Performance Measure.
* WebRipper

1. **Vulnerability Scanning**

Attackers seek to find vulnerabilities that can be exploited to be used as an entrance to the Target Website. Patch Tuesday attack Wednesday is typical for attackers who dive into a zero-day attack to gain quick win access to The Target system. Following tools can be used to find vulnerabilities:

* Tenable Nessus
* Nikto2
* Netsparker
* OpenVAS
* Acunetix
* Nmap
* OpenSCAP

1. **Session hijacking**

A session hijacking attack exploits a session-token generation mechanism or token security controls so that the attacker can establish an unauthorized connection with a target server. Session Hijacking would include different processes such as Sniffing, Monitoring, session desynchronization, session ID prediction, and command injection. Various methodologies can be utilized for compromising sessions IDs as

* Packet Sniffing tools as Wireshark
* Man-in-the-middle \(MITM\) Attack.
* XSS Attack
* CSRF Attack
* Session Replay Attack

1. **Website Password Hacking**

Attackers use password-cracking ****methods like brute force attacks, hybrid attacks, dictionary attacks, and so on, to crack web server's password. Following, examples of password cracking tools

* Wfuzz
* Cain & Abel.
* John the Ripper.
* THC Hydra.

As we have expressed typical methodologies used for attacking web applications. In next Section we would go through Common Countermeasures to protect Web Application.

* Periodic review and assessments on public information about web services and technologies used. Such information can be located at search engines, social networking, or professional networking websites.
* Awareness training for users to train them how to deal with information in a protected way, expressing information classifications, social engineering common approaches and highlighting Due care concepts.
* Disable unused services on publicly accessible web services
* Follow Secure Development Life Cycle for application development which ensures applied security baseline integrated with app functionality.
* Perform Due Diligence by having Security assessment or penetration testing on newly published and periodic ones in currently deployed services.
* Periodic Vulnerability assessment
* Patching system to keep systems up to date.
* Implement a Web Application Firewall \(Reverse Proxy\) to serve your public web applications
* Enable Input Validation based on Size, length, or characters.
* Ensure Encrypted tunnel TLS as well as encrypted cookies.
* Enable CORS Cross-Origin-Resource-Sharing \(X-origin\) Header
* File input Validation based on file type, Size
* Integrate WAF Proxy with the anti-malware solution to scan files before uploading to the server.
* Audit and Logging activity
* Replace default URL response error pages
* Disable Client-Side Scripting.
* Decrypt inbound and outbound traffic with NGFW capabilities \(IPS, Anti-Malware\)
* Logging Correlation \(SEIM\)

References

[https://info-savvy.com/6-quick-methodology-for-web-server-attack/ \(Links to an external site.\)](https://info-savvy.com/6-quick-methodology-for-web-server-attack/)

[https://0xsanz.medium.com/web-enumeration-methodology-8b44e52730d6 \(Links to an external site.\)](https://0xsanz.medium.com/web-enumeration-methodology-8b44e52730d6)

[https://shehackske.medium.com/information-gathering-for-website-hacking-1682ed67f29a](https://shehackske.medium.com/information-gathering-for-website-hacking-1682ed67f29a)

