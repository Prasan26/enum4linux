# Volatile and non-volatile information

Week 4 Discussion – Forensic Collection of Volatile and Non-Volatile Information from Windows Systems - Andrew Merkle – ECCU 2021 Term 3

CIS 406 – System Forensics, Investigation, and Response - Instructor Sandro Tuccinardi

The objective for this assignment is “_Discusses how forensic investigators can collect volatile and non-volatile information from Windows systems.”_

According to the Internet Security Glossary IETF 2828 \(Shirey, 2000\), a security incident is “a security-relevant system event in which the system's security policy is disobeyed or otherwise breached.” The Guidelines for Evidence Collection and Archiving IETF 3228 \(Brezinski & Killalea, 2002\) states that “If evidence collection is done correctly, it is much more useful in apprehending the attacker, and stands a much greater chance of being admissible in the event of a prosecution.”

The goal of the digital forensic investigator is to gather evidence without changing it in order to perform a fair and impartial analysis. However, it is one of the laws of physics that to measure something, one must interact with it. In the study of quantum mechanics, it is well understood that by measuring a particle, the particle momentum is changed. The same principle is true with regard to a computer system. By interacting with it, even in seemingly trivial ways, one or more changes will be imparted. By loading a forensic utility, some small part of the memory and CPU registers will be changed. Even moving the mouse or connecting a USB drive will change something. Yet the data that is in the volatile memory of the system, which would be lost if the system were powered off, is some of the most important evidence to be gathered. Therefore, in addition to adhering to legal and ethical principles, the investigator must also approach this task scientifically, with a strategy that will minimize any impact the data gathering may have on the integrity of the evidence. Plan the investigation. Assemble a toolkit. Then collect the evidence according to the order of volatility.

For a system running Microsoft Windows, EC-Council \(2021\) notes a number of items that should be gathered and the utility programs that can be executed to do so, which often may be combined and executed by a script to automate and expedite the process since time is of the essence. Each command line utility has a number of different parameters that can be set on the command line, and which should be configured by the examiner to collect information pertaining to the investigation. Some commands might be run multiple times with different settings:

| system time | date /t & time /t |  |
| :--- | :--- | :--- |
| users logged on | psloggedon |  |
|  | net sessions |  |
|  | logonsessions -c -p |  |
| files that are open | net file |  |
| files open via remote access | NetworkOpenedFiles | [https://www.nirsoft.netLinks to an external site.](https://www.nirsoft.net/) |
| network information | nbtstat |  |
|  | netstat |  |
| process and port info | tasklist |  |
|  | pslist |  |
|  | listdlls |  |
|  | handle |  |
|  | netstat |  |
|  | Process Explorer \(GUI\) |  |
|  | ProcDump |  |
|  | Process Dumper | [https://github.comLinks to an external site.](https://github.com/) |
| network status | Ipconfig |  |
|  | PromiscDetect |  |
|  | Promqry |  |
| print spool information | C:\Windows\System32\spool\PRINTERS folder |  |
|  | Free Hex Editor Neo |  |
|  | UCCHECK |  |
| clipboard | Free Clipboard Viewer | [https://freeclipboardviewer.comLinks to an external site.](https://freeclipboardviewer.com/) |
| services and drivers | wmic |  |
| history of commands | doskey /history |  |
| resources shared locally | net share |  |

\(List adapted from EC-Council, 2021\)

Following the run of a script \(or of individual utilities\) for capture of the foregoing volatile information, a memory capture image should be made for subsequent analysis, which can contain the memory swap also. The memory image can be analyzed by a number of free or commercial utilities. Following the collection of volatile data from an evidence machine, a forensic image of hard drives and removable media may be made which can then be analyzed as well to recognize important databases, browser data, user search terms, information about devices connected to the system. Slack space, hidden partitions, and various other non-volatile data may contain useful evidence. File carving may be performed to recover files that had been deleted or lost.

Consideration should be given, if at all possible, to gathering the evidence in the order presented by Brezinski & Killalea \(2002\) in their Guidelines for Evidence Collection and Archiving:

* registers, cache
* routing table, arp cache, process table, kernel statistics, memory
* temporary file systems
* disk
* remote logging and monitoring data that is relevant to the system in question
* physical configuration, network topology
* archival media

References

Balaji N. \(2019, August 12\). _Incident response tools list for hackers and penetration testers._ GBHackers On Security. [https://gbhackers.com/cyber-incident-response-tools/Links to an external site.](https://gbhackers.com/cyber-incident-response-tools/)

Brezinski, D., & Killalea, T. \(2002, February\). _Guidelines for evidence collection and archiving - RFC 3227 - BCP 55._ Network Working Group - Internet Engineering Task Force. [https://www.ietf.org/rfc/rfc3227.txtLinks to an external site.](https://www.ietf.org/rfc/rfc3227.txt)

Computer Forensics Recruiter \(CFR\). \(2016, June 29\). _Order of volatility._ [https://www.computer-forensics-recruiter.com/order-of-volatility/Links to an external site.](https://www.computer-forensics-recruiter.com/order-of-volatility/)

Dhanunjaya. \(2016, April 8\). _Collecting volatile and non-volatile data._ eForensics. [https://e4n6.wordpress.com/2016/04/08/collecting-volatile-and-non-volatile-data/Links to an external site.](https://e4n6.wordpress.com/2016/04/08/collecting-volatile-and-non-volatile-data/)

EC-Council. \(2020\). Certified Ethical Hacker \(CEH\) Version 11 eBook w/ iLabs \(Volumes 1 through 4\). \[VitalSource Bookshelf 9.2.1\].  Retrieved from vbk://9781635675160

EC-Council. \(2021\). Computer Hacking Forensics Investigator \(CHFI\) Version 10, 10th Edition. \[VitalSource Bookshelf 9.2.1\].  Retrieved from vbk://9781635676969

Kent, K., Chevalier, S., Grance, T., & Dang, H. \(2006, August\). _Guide to integrating forensic techniques into incident response._ NIST Technical Series Publications - National Institute of Standards and Technology. [https://nvlpubs.nist.gov/nistpubs/legacy/sp/nistspecialpublication800-86.pdfLinks to an external site.](https://nvlpubs.nist.gov/nistpubs/legacy/sp/nistspecialpublication800-86.pdf)

Kim, D. \(2016\). Fundamentals of Information Systems Security, 3rd Edition. \[VitalSource Bookshelf 9.2.1\]. Retrieved from vbk://9781284128567

Mazerik, R. \(2013, December 30\). _Forensic investigation on Windows machines._ Infosec Resources - Digital Forensics. [https://resources.infosecinstitute.com/topic/forensic-investigation-windows-machines/Links to an external site.](https://resources.infosecinstitute.com/topic/forensic-investigation-windows-machines/)

Nolan, R., O’Sullivan, C., Branson, J., & Waits, C. \(2005, March\). _First responders guide to computer forensics._ SEI Digital Library - Carnegie Mellon Software Engineering Institute. [https://resources.sei.cmu.edu/asset\_files/Handbook/2005\_002\_001\_14429.pdfLinks to an external site.](https://resources.sei.cmu.edu/asset_files/Handbook/2005_002_001_14429.pdf)

SEI/CERT. \(2016\). _Volatile data collection._ Cybersecurity and Infrastructure Security Agency Federal Virtual Training Environment - CISA FedVTE. [https://fedvte.usalearning.gov/courses/CSI/course/videos/pdf/CSI\_D01\_S05\_T01\_STEP.pdfLinks to an external site.](https://fedvte.usalearning.gov/courses/CSI/course/videos/pdf/CSI_D01_S05_T01_STEP.pdf)  
Lecture slides provided by and © 2016 Carnegie Mellon University Software Engineering Institute. CERT® is a registered mark owned by Carnegie Mellon University.  
The Federal Virtual Training Environment \(FedVTE\) provides free online cybersecurity training to federal, state, local, tribal, and territorial government employees, federal contractors, and US military veterans \([https://fedvte.usalearning.gov/coursecat\_external.phpLinks to an external site.](https://fedvte.usalearning.gov/coursecat_external.php)\).

Shipley, T. G., & Reeve, H. R. \(2006\). _Collecting evidence from a running computer: A technical and legal primer for the justice community._ SEARCH \| The National Consortium for Justice Information and Statistics. [https://search.org/files/pdf/CollectEvidenceRunComputer.pdfLinks to an external site.](https://search.org/files/pdf/CollectEvidenceRunComputer.pdf)  
SEARCH, the National Consortium for Justice Information and Statistics, is a nonprofit organization governed by a Membership Group of governor appointees from the 50 States, the District of Columbia, and the territories. SEARCH—an acronym for System for the Electronic Analysis and Retrieval of Criminal Histories—began as a project in 1969 funded by the Law Enforcement Assistance Administration \(LEAA\).

Shirey, R. \(2000, May\). _Internet security glossary - RFC 2828 - FYI 36._ Network Working Group - Internet Engineering Task Force. [https://www.ietf.org/rfc/rfc2828.txtLinks to an external site.](https://www.ietf.org/rfc/rfc2828.txt)

