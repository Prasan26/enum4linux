---
description: >-
  Give your opinion on OS banner grabbing and explain how to identify target
  system OS.
---

# WEEK 2

Banner grabbing is a technique used by hackers and security team to gain information about computer system on network and services running on its ports.This technique can gain information from banners and configurable text-based welcome screens from network hosts.

These banners and network hosts generally contain information about the system.  Few examples of service ports that are used for the Banner Grabbing technique are HTTP \(TCP/80\), FTP \(TCP/20,21\), and SMTP \(TCP/25\)

There are two types of techniques available to perform Banner grabbing; Active and Passive.

* Active: This is the popular one and most widely used. Hackers intent to sent packets to remote host and analyze responses.
* Passive: it could include Sniffing the network traffic, then analyze it with Wireshark. Hackers deploy intermediate software/Website as a gateway to prevent a direct connection with target. These Tools collect website error pages, Header Cookies or Website file type extensions, then analyze to determine running service and OS type.

Grabbing tools include; NMAP, Netcat, Netcraft, Telnet, cURL, Wget.

<table>
  <thead>
    <tr>
      <th style="text-align:left">Telnet</th>
      <th style="text-align:left"></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Wget</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">cURL</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">netcat</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">NMAP</td>
      <td style="text-align:left">
        <p>nmap -sV 10.0.1.201</p>
        <p>nmap -O 10.0.1.201</p>
      </td>
    </tr>
  </tbody>
</table>

As a security practitioner, you should raise flag for the organization in order to reduce the attack surface and pervent banner grapping as

* Restrict access to service on network based on Need to know and least privilege concepts
* Shutdown unused ports or services running on network hosts
* Customize system default configurations, whatever password, banners, default ports, default usernames, error pages ...etc.
* Keep system patched and up to date, and always remember this "Patch Tuesday, exploit Wednesday".
* Remove unnecessary headers, Change default cookie names, hide server files extensions, review app source code to remove information that can esily learn the used framework and its version.

References:

Ho, L. Y. \(n.d.\). 3.4 Banner Grabbing. 3.4 Banner Grabbing · CEH\_v9. [https://ktflash.gitbooks.io/ceh\_v9/content/34\_ceh\_scanning\_methodology\_-\_banner\_grabbing.html \(Links to an external site.\)](https://ktflash.gitbooks.io/ceh_v9/content/34_ceh_scanning_methodology_-_banner_grabbing.html).

Banner Grabbing: In 3 Easy Points. Jigsaw Academy. \(2021, January 1\). [https://www.jigsawacademy.com/blogs/cyber-security/banner-grabbing/ \(Links to an external site.\)](https://www.jigsawacademy.com/blogs/cyber-security/banner-grabbing/).

WSTG - Latest. OWASP. \(n.d.\). [https://owasp.org/www-project-web-security-testing-guide/latest/4-Web\_Application\_Security\_Testing/01-Information\_Gathering/08-Fingerprint\_Web\_Application\_Framework \(Links to an external site.\)](https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/01-Information_Gathering/08-Fingerprint_Web_Application_Framework).

