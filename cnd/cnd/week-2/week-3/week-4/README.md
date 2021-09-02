---
description: >-
  Identify necessary countermeasures that should be performed by the users for
  preventing their systems from various malware threats.
---

# WEEK 4



Security countermeasures categories include; administrative, physical and Logical \(technical\) controls.

* **administrative controls** include an organization\`s policy, guidelines and procedures. These controls states an organization requirements to provide a secure service such as  security policy , User awareness training,  acceptable use policy, etc. Mainly of these administrative controls would be based on regulations and security best practices.
* **Physical control**s include tangible security controls as CCTV systems, guards, fences, dogs and other. It is the base corner for security as without physical security you can secure nothing.
* **Logical controls** include technical controls as Firewalls, Host Intrusion Detection systems, Anti-Malware Software and others.

after we have defined each type of control. From a security design perspective you should use all type of controls to secure an organization systems. the secret word here would be defense-in-depth.

![DIP.JPG](https://eccouncil.instructure.com/users/1805/files/476056/preview?verifier=KapwqVJKP7Ui1Ayd9xyxPQ7AtczKaCaVgUu2IQI2)

you should rely on multiple security layers as in case one fails, other can provide a adequate protection. Also from security countermeasure cycle, there would be different types of countermeasure or controls as detective, preventive and corrective.

* **Detective controls** mainly used for detecting a threat on your organization as Security Information and Event Management SIEM, Intrusion Detection System IDS, Behavior and Network analysis systems.
* **Preventive control**s mainly used for blocking a threat as Firewalls, Intrusion Prevention systems, antivirus software and others.
* **Corrective controls** mainly used for fix and restoration for service or host after attack is already took a place as antivirus try to remove a virus from an endpoint or restoring a backup after ransomware has encrypted your files.

After we have explained different categories of controls and its types. Our focus would be how to protect our systems from various malware threats. First we should able to define what is a Malware!. A Malware is an malicious file that can cause damage on a computer system and allow limited or full unauthorized control to the malware creator such as theft or fraud. Malware is a general acronym which cover all types of malicious files as Trojans, virus, botnets, ransomware, keyloggers, rootkits, etc.

in next section we would explore different security controls based on security best practices to protect against malwares.

1. Clear Security policy states Internet access policy for each department including allowed web sites, allowed file types downloads,etc.
2. Clear Security policy for Security posture for machines allowed to access the network including last patch updates, antivirus installed, domain Join, etc.
3. Clear Security policy for Privilege Access machines \(PAW\) including preventing internet access, USB , different username than regular one used for accessing web and email services.
4. Clear Security policy for Patching and vulnerability assessment including max time to apply patches, regular/periodic vulnerability scan based on different scopes.
5. Clear Security Policy for email service as Blocking specific attachment file types, attachment sandbox scanning, etc.
6. Clear Security policy for Network access includes network segmentation, Dot1x enforcement, Machine\`s security posture checks, etc.
7. Clear Security policy for user-awareness training includes mandatory attendance, explaining different types of attacks and its impact on organization, final evaluation criteria, periodic simulation attack as phishing, etc.
8. Clear Security policy for Physical security access to prevent unauthorized person in specific area as it may implant physical keylogger or a malicious USB

Once we have endorsement from top management, we would be able to apply different countermeasure including.

1. **Network Segmentation** for users access \(IT, Marketing, Help-desk, etc.\)
2. **Perimeter Next Generation Firewalls** to inspect inbound and outbound traffic \(Decryption is highly required\) + Intrusion prevention systems
3. **Web Security system** to filter and inspect web traffic for organization \(Decryption is highly required\)
4. **Email Security system** to protect organizations email service \(Cisco ESA\)
5. Perimeter NGFW + Email Security system + Web Security system **must be all integrated into Dynamic Malware analysis** Service
6. **Dynamic Malware Analysis** as Cisco ThreatGrid, Paloalto Wildfire \(On-Premise or Cloud\)
7. **Security Information and Event Management systems** for Logs Correlation and generation of Indication of Compromise IOC.
8. **Cloud integration with Threat Detection services** as Cisco Talos, Kaspersky, etc. this service would keep you up to date with Malicous IPs , URLs, Domains and File hashes.
9. **Host Intrusion Detection system** on Users\` endpoints
10. **Anti-Malware software** on Users endpoints
11. **Patch management System** to deploy periodic patches and keep system up to date.
12. **Vulnerability assessment systems** as Tenable to scan network/hosts periodically and insight us about environment security posture state.
13. **Group Policy orchestration GPO for corporate devices** to define allowed software, blocking USB usage, block unused services, etc.
14. **Mobile Device management for BYOD devices** to define whitelist applications, block specific services, etc.
15. **Backup System** for periodic backup for servers and workstations. in case of ransomware, you can roll-back to a well steady state.
16. **User Awareness Training** for Users, Management and TOP Management

{% tabs %}
{% tab title="First Tab" %}
**Malware Threats Prevention**

To save your gadgets from being inflamed with malware, there are numerous steps you may take:

1. Install Anti-virus software program\(Strawbridge, 2018\)

One of the essential approaches to guard towards malware is to put in an anti-virus software program. The anti-virus software program will protect your tool from the malicious software program that poses a risk to the system. It will experiment your laptop to come across and ease the malware and offer automated updates to offer improved safety towards newly created viruses.

1. Regularly replace software program

 In addition to putting in an anti-virus software program, it's essential to make sure that your software program is often up to date to forestall attackers from getting access to your laptop via vulnerabilities in older and old systems.

1. Only purchase Apps from relied-on assets.

 Buying apps from natural assets reduces the danger of your tool being inflamed with malware. Big manufacturers will take excellent care to make sure they do now no longer harm their recognition with the aid of using dispensing malware. To take a look at the authenticity of a source, you may look at the real name, a listing of posted apps, and get in touch with info withinside the app description withinside the Google Play or Apple app store.

1. Don't click on suspicious hyperlinks or download attachments from unknown assets. Phishing stays the perfect manner for hackers to put in malware for your tool. Phishing scams trick human beings into starting emails or clicking on a hyperlink which can seem to return from a good enterprise or professional source. The hyperlink might also additionally direct you to a faux internet site in which you're caused to go into your info or take you to an internet site that without delay infects your laptop with malware. If in doubt, don't click on the hyperlink.
2. Install Firewall Another manner to guard your tool from malware is to apply a firewall. A firewall prevents malicious assaults with the aid of using blocking off all unauthorized get entry to or from a personal laptop network. In addition to anti-virus software programs, a firewall gives a further barrier towards malware, decreasing the danger of attack.
3. Back up information often

 It's critical to return up often to make certain that you may nevertheless retrieve all of your treasured information and documents if your laptop is inflamed with malware. This will assist mitigate any harm and make particular which you aren't held sufferer to a ransomware attack. Phishing is the primary reason for all cyber-assaults and maintains to show one of the most straightforward approaches to thieve treasured information and supply malware. MetaPhish has been created to offer adequate protection towards those threats and permits businesses to discover simply how prone their corporation is to Phishing. If you would love to learn extra approximately how MetaPhish may guard your enterprise, then touch us for additional information.

## References

Strawbridge, G. \(2018, August 28\). _Cyber Security Awareness, Phishing and Ransomware, Security Awareness Training_ . Retrieved from MetaCompliance: https://www.metacompliance.com/blog/what-is-malware-and-how-to-prevent-against-it/
{% endtab %}

{% tab title="Second Tab" %}

{% endtab %}
{% endtabs %}

