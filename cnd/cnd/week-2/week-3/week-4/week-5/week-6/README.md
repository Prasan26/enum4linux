---
description: Discuss the role of the honeypots in safeguarding the organization’s network.
---

# WEEK 6

Honeypot is a crucial defense layer in network security architecture. Honeypots appear to be a fragile entry point into an organization network to distract attackers from looking at other sensitive systems. They support us in detecting an early sign of attack, define details of the attacker, and used methods. Honeypot is a system that is implemented to be exploited, hacked, infected with malicious files, and abused by attackers. it is actually made for this purpose.

Honeypots may be single or a network of honeypots. Honeypots are commonly located at isolated DMZ segments behind Firewall. Honeypots often use hardened Operation systems where extra security measures are taken to minimize their exposure to threats. At the same time, it should appear to offer attackers exploitable vulnerabilities as SMB used with WannaCry Ransomware.

 Based on design and deployment, there are two main types of honeypots:

* **Research honeypots** perform a close analysis of hacker activity and aim to discover how hackers develop and progress to learn how to better protect systems against them.
* **Production honeypots** are usually deployed inside production networks alongside production servers; the honeypot acts as a decoy, drawing intruders away from the production network as part of the intrusion detection system \(IDS\). This approach ultimately gives administrators time to assess the threat level and mitigate any vulnerabilities in their existing production systems.

Based on the function used, there are different Honeypot types :

* **Pure Honeypot:** A full-scale production replication system that can run on other servers. It has comprehensive sensors and carries dummy “confidential” data and user details.
* **High-Interaction Honeypot:** It is used by the security analyst to observe the attacker’s techniques and behavior pattern. These types of honeypots are quite resource-intensive and demand more maintenance but can deliver worthwhile findings.
* **Mid-Interaction Honeypot:** They do not possess their own operating system and are primarily used to confuse the attackers to buy some time for the security team to react to the breach.
* **Low-Interaction Honeypot:** This form of **honeypot in network security** is widely deployed while creating a production environment. It is used for advanced warning spotting mechanisms. They are pretty simple to deploy and maintain.

Based on the Technology involved, there are different Honeypot types:

* **Malware Honeypots:** It is known to replicate and use attack vectors to identify malware. One example is the Ghost USB honeypot meant to safeguard the machine from malware spread through USB.
* **Spam Honeypots:** It is used to simulate open proxies and mail relays. It detects and blocks the large number of spam emails dispatched by spammers.
* **Database Honeypots:** It helps in creating decoy databases. These types of honeypots are effective against activities like SQL injections that frequently go untraced by the firewalls.
* **Client Honeypots:** It helps trace out malicious servers that are primarily responsible for attacking clients. It functions over virtualization technology and implements a containment strategy to curtail the risk imposed on the research team.
* **Honeynets:** It is a single system comprising of multiple **honeypots in network security**. The purpose of the honeynets is to tactically track down the motives and methods of the attacker, simultaneously containing all sorts of outbound and inbound traffic.

The following are some of the significant benefits of a honeypot:

*  **Ability to break/ slow attackers down:** While scanning your network, attackers always seek misconfiguration and vulnerable devices. An encounter with the honeypot renders you the chance to investigate and restrain the attack on time.
* **Unambiguous in Approach:** Honeypot does provide you with a precise alert and location of the breach. It does help you out with identifying the loopholes as well as the invasion threat without scanning unnecessary areas and wasting time.
*  **Easy to Install and demand low-maintenance:** Modern honeypots are easy to download and install. They also require low-maintenance time and cost
* **Encryption circumvention.** Honeypots capture malicious activity, even if an attacker is using encryption.
* **Real data collection \(Intelligence Data\).** Honeypots collect data from actual attacks and other unauthorized activities, providing analysts with a rich source of helpful information.
* **Improve Security Posture**
* **Identify Attackers Profile**

Disadvantages

* **Limited data.** Honeypots only collect information when an attack occurs. Zero attempts to access the honeypot means there is no data to analyze.
* **Isolated network.** Malicious traffic that has been captured is only collected when an attack targets the honeypot network; if attackers suspect a network is a honeypot, they will avoid it.
* **Distinguishable.** Honeypots are often different from legitimate production systems, which means experienced hackers can usually differentiate a production system from a honeypot system using system fingerprinting techniques.
* **Put production systems at risk.** Although they are isolated from the actual network, they do eventually connect in some way to enable administrators to collect the information they contain. A high-interaction honeypot is generally considered riskier than a low-interaction one because it aims to entice hackers to gain root access.

References

[https://ipwithease.com/understanding-types-and-benefits-of-honeypot-in-network-security/ \(Links to an external site.\)](https://ipwithease.com/understanding-types-and-benefits-of-honeypot-in-network-security/)

[https://searchsecurity.techtarget.com/definition/honey-pot \(Links to an external site.\)](https://searchsecurity.techtarget.com/definition/honey-pot)

[https://www.informit.com/articles/article.aspx?p=30489&seqNum=3](https://www.informit.com/articles/article.aspx?p=30489&seqNum=3)

