# Incident Response List 🛡️

## Overview 🌐
This repository contains a list of tools, techniques, and resources for incident response (IR) in cybersecurity. It provides detailed insights into the incident response process, including detection, containment, and recovery.

## Table of Contents 📚
1. [Tools 🧰](##tools)
2. [Techniques 🛠️](##techniques)
3. [Log Analysis Tools](##log-analysis-tools)
4. [Memory Analysis Tools](##memory-analysis-tools)
5. [Memory Imaging Tools](##memory-imaging-tools)
6. [OSX Evidence Collection](##osx-evidence-collection)
7. [Other Lists](##other-lists)
8. [Other Tools](##other-tools)
9. [Playbooks](##playbook)
10. [Process Dump Tools](##process-dump-tools)
11. [Sandboxing/Reversing Tools](##sandboxing-tools)
12. [Scanner Tools](##scanner-tools)
13. [Timeline Tools](##timeline-tools)
14. [Windows Evidence Collection](##windows-evidence-collection)
15. [Resources 📖](##resources)
16. [Useful Links 🌍](#useful-links)

---

## Tools 🧰
- **[Wireshark](https://www.wireshark.org/)**: A network protocol analyzer used for network traffic analysis. Great for identifying malicious traffic in packet captures (PCAPs).
- **[Sysinternals Suite](https://docs.microsoft.com/en-us/sysinternals/)**: A collection of tools for monitoring and managing Windows environments, useful for investigating malware behavior and system forensics.
- **[Volatility](https://www.volatilityfoundation.org/)**: A memory forensics tool that allows for the analysis of memory dumps to uncover malware and other suspicious activities.

## Techniques 🛠️
- **Network Traffic Analysis**: Monitor network traffic for signs of anomalies, such as unusual protocols or traffic spikes, to identify malicious activity.
- **Log Analysis**: Analyze logs from various sources (e.g., system, firewall, web server) to detect signs of an attack, such as failed login attempts, privilege escalation, or suspicious file modifications.
- **Memory Analysis**: Use memory analysis tools to examine live memory dumps or system snapshots to uncover evidence of running malware or suspicious processes.

## Log Analysis Tools

* [AppCompatProcessor](https://github.com/mbevilacqua/appcompatprocessor) - AppCompatProcessor has been designed to extract additional value from enterprise-wide AppCompat / AmCache data beyond the classic stacking and grepping techniques.
* [APT Hunter](https://github.com/ahmedkhlief/APT-Hunter) - APT-Hunter is Threat Hunting tool for windows event logs.
* [Chainsaw](https://github.com/countercept/chainsaw) - Chainsaw provides a powerful ‘first-response’ capability to quickly identify threats within Windows event logs.
* [Event Log Explorer](https://eventlogxp.com/) - Tool developed to quickly analyze log files and other data.
* [Event Log Observer](https://lizard-labs.com/event_log_observer.aspx) - View, analyze and monitor events recorded in Microsoft Windows event logs with this GUI tool.
* [Hayabusa](https://github.com/Yamato-Security/hayabusa) - Hayabusa is a Windows event log fast forensics timeline generator and threat hunting tool created by the Yamato Security group in Japan.
* [Kaspersky CyberTrace](https://support.kaspersky.com/13850) - Threat intelligence fusion and analysis tool that integrates threat data feeds with SIEM solutions. Users can immediately leverage threat intelligence for security monitoring and incident report (IR) activities in the workflow of their existing security operations.
* [Log Parser Lizard](https://lizard-labs.com/log_parser_lizard.aspx) - Execute SQL queries against structured log data: server logs, Windows Events, file system, Active Directory, log4net logs, comma/tab separated text, XML or JSON files. Also provides a GUI to Microsoft LogParser 2.2 with powerful UI elements: syntax editor, data grid, chart, pivot table, dashboard, query manager and more.
* [Lorg](https://github.com/jensvoid/lorg) - Tool for advanced HTTPD logfile security analysis and forensics.
* [Logdissect](https://github.com/dogoncouch/logdissect) - CLI utility and Python API for analyzing log files and other data.
* [LogonTracer](https://github.com/JPCERTCC/LogonTracer) - Tool to investigate malicious Windows logon by visualizing and analyzing Windows event log.
* [Sigma](https://github.com/SigmaHQ/sigma) - Generic signature format for SIEM systems already containing an extensive ruleset.
* [StreamAlert](https://github.com/airbnb/streamalert) - Serverless, real-time log data analysis framework, capable of ingesting custom data sources and triggering alerts using user-defined logic.
* [SysmonSearch](https://github.com/JPCERTCC/SysmonSearch) - SysmonSearch makes Windows event log analysis more effective and less time consuming by aggregation of event logs.
* [WELA](https://github.com/Yamato-Security/WELA) - Windows Event Log Analyzer aims to be the Swiss Army knife for Windows event logs.
* [Zircolite](https://github.com/wagga40/Zircolite) - A standalone and fast SIGMA-based detection tool for EVTX or JSON.

## Memory Analysis Tools

* [AVML](https://github.com/microsoft/avml) - A portable volatile memory acquisition tool for Linux.
* [Evolve](https://github.com/JamesHabben/evolve) - Web interface for the Volatility Memory Forensics Framework.
* [inVtero.net](https://github.com/ShaneK2/inVtero.net) - Advanced memory analysis for Windows x64 with nested hypervisor support.
* [LiME](https://github.com/504ensicsLabs/LiME) - Loadable Kernel Module (LKM), which allows the acquisition of volatile memory from Linux and Linux-based devices, formerly called DMD.
* [MalConfScan](https://github.com/JPCERTCC/MalConfScan) - MalConfScan is a Volatility plugin extracts configuration data of known malware. Volatility is an open-source memory forensics framework for incident response and malware analysis. This tool searches for malware in memory images and dumps configuration data. In addition, this tool has a function to list strings to which malicious code refers.
* [Memoryze](https://www.fireeye.com/services/freeware/memoryze.html) - Free memory forensic software that helps incident responders find evil in live memory. Memoryze can acquire and/or analyze memory images, and on live systems, can include the paging file in its analysis.
* [Memoryze for Mac](https://www.fireeye.com/services/freeware/memoryze.html) - Memoryze for Mac is Memoryze but then for Macs. A lower number of features, however.
* [MemProcFS] (https://github.com/ufrisk/MemProcFS) - MemProcFS is an easy and convenient way of viewing physical memory as files in a virtual file system.
* [Orochi](https://github.com/LDO-CERT/orochi) - Orochi is an open source framework for collaborative forensic memory dump analysis.
* [Rekall](http://www.rekall-forensic.com/) - Open source tool (and library) for the extraction of digital artifacts from volatile memory (RAM) samples.
* [Volatility](https://github.com/volatilityfoundation/volatility) - Advanced memory forensics framework.
* [Volatility 3](https://github.com/volatilityfoundation/volatility3) - The volatile memory extraction framework (successor of Volatility)
* [VolatilityBot](https://github.com/mkorman90/VolatilityBot) - Automation tool for researchers cuts all the guesswork and manual tasks out of the binary extraction phase, or to help the investigator in the first steps of performing a memory analysis investigation.
* [VolDiff](https://github.com/aim4r/VolDiff) - Malware Memory Footprint Analysis based on Volatility.
* [WindowsSCOPE](http://www.windowsscope.com/windowsscope-cyber-forensics/) - Memory forensics and reverse engineering tool used for analyzing volatile memory offering the capability of analyzing the Windows kernel, drivers, DLLs, and virtual and physical memory.


## Memory Imaging Tools

* [Belkasoft Live RAM Capturer](http://belkasoft.com/ram-capturer) - Tiny free forensic tool to reliably extract the entire content of the computer’s volatile memory – even if protected by an active anti-debugging or anti-dumping system.
* [Linux Memory Grabber](https://github.com/halpomeranz/lmg/) - Script for dumping Linux memory and creating Volatility profiles.
* [MAGNET DumpIt](https://www.magnetforensics.com/resources/magnet-dumpit-for-windows) - Fast memory acquisition tool for Windows (x86, x64, ARM64). Generate full memory crash dumps of Windows machines.
* [Magnet RAM Capture](https://www.magnetforensics.com/free-tool-magnet-ram-capture/) - Free imaging tool designed to capture the physical memory of a suspect’s computer. Supports recent versions of Windows.
* [OSForensics](http://www.osforensics.com/) - Tool to acquire live memory on 32-bit and 64-bit systems. A dump of an individual process’s memory space or physical memory dump can be done.

## OSX Evidence Collection

* [Knockknock](https://objective-see.com/products/knockknock.html) - Displays persistent items(scripts, commands, binaries, etc.) that are set to execute automatically on OSX.
* [macOS Artifact Parsing Tool (mac_apt)](https://github.com/ydkhatri/mac_apt) - Plugin based forensics framework for quick mac triage that works on live machines, disk images or individual artifact files.
* [OSX Auditor](https://github.com/jipegit/OSXAuditor) - Free Mac OS X computer forensics tool.
* [OSX Collector](https://github.com/yelp/osxcollector) - OSX Auditor offshoot for live response.
* [The ESF Playground](https://themittenmac.com/the-esf-playground/) - A tool to view the events in Apple Endpoint Security Framework (ESF) in real time.

## Other Lists

* [Awesome Event IDs](https://github.com/stuhli/awesome-event-ids) - Collection of Event ID resources useful for Digital Forensics and Incident Response.
* [Awesome Forensics](https://github.com/cugu/awesome-forensics) - A curated list of awesome forensic analysis tools and resources.
* [Didier Stevens Suite](https://github.com/DidierStevens/DidierStevensSuite) - Tool collection
* [Eric Zimmerman Tools](https://ericzimmerman.github.io/) - An updated list of forensic tools created by Eric Zimmerman, an instructor for SANS institute.
* [List of various Security APIs](https://github.com/deralexxx/security-apis) - Collective list of public JSON APIs for use in security.

## Other Tools

* [Cortex](https://thehive-project.org) - Cortex allows you to analyze observables such as IP and email addresses, URLs, domain names, files or hashes one by one or in bulk mode using a Web interface. Analysts can also automate these operations using its REST API.
* [Crits](https://crits.github.io/) - Web-based tool which combines an analytic engine with a cyber threat database.
* [Diffy](https://github.com/Netflix-Skunkworks/diffy) - DFIR tool developed by Netflix's SIRT that allows an investigator to quickly scope a compromise across cloud instances (Linux instances on AWS, currently) during an incident and efficiently triaging those instances for followup actions by showing differences against a baseline.
* [domfind](https://github.com/diogo-fernan/domfind) - Python DNS crawler for finding identical domain names under different TLDs.
* [Fileintel](https://github.com/keithjjones/fileintel) - Pull intelligence per file hash.
* [HELK](https://github.com/Cyb3rWard0g/HELK) - Threat Hunting platform.
* [Hindsight](https://github.com/obsidianforensics/hindsight) - Internet history forensics for Google Chrome/Chromium.
* [Hostintel](https://github.com/keithjjones/hostintel) - Pull intelligence per host.
* [imagemounter](https://github.com/ralphje/imagemounter) - Command line utility and Python package to ease the (un)mounting of forensic disk images.
* [Kansa](https://github.com/davehull/Kansa/) - Modular incident response framework in PowerShell.
* [MFT Browser](https://github.com/kacos2000/MFT_Browser) - MFT directory tree reconstruction & record info.
* [Munin](https://github.com/Neo23x0/munin) - Online hash checker for VirusTotal and other services.
* [PowerSponse](https://github.com/swisscom/PowerSponse) - PowerSponse is a PowerShell module focused on targeted containment and remediation during security incident response.
* [PyaraScanner](https://github.com/nogoodconfig/pyarascanner) - Very simple multi-threaded many-rules to many-files YARA scanning Python script for malware zoos and IR.
* [rastrea2r](https://github.com/rastrea2r/rastrea2r) - Allows one to scan disks and memory for IOCs using YARA on Windows, Linux and OS X.
* [RaQet](https://raqet.github.io/) - Unconventional remote acquisition and triaging tool that allows triage a disk of a remote computer (client) that is restarted with a purposely built forensic operating system.
* [Raccine](https://github.com/Neo23x0/Raccine) - A Simple Ransomware Protection
* [Stalk](https://www.percona.com/doc/percona-toolkit/2.2/pt-stalk.html) - Collect forensic data about MySQL when problems occur.
* [Scout2](https://nccgroup.github.io/Scout2/) - Security tool that lets Amazon Web Services administrators assess their environment's security posture.
* [Stenographer](https://github.com/google/stenographer) - Packet capture solution which aims to quickly spool all packets to disk, then provide simple, fast access to subsets of those packets. It stores as much history as it possible, managing disk usage, and deleting when disk limits are hit. It's ideal for capturing the traffic just before and during an incident, without the need explicit need to store all of the network traffic.
* [sqhunter](https://github.com/0x4d31/sqhunter) - Threat hunter based on osquery and Salt Open (SaltStack) that can issue ad-hoc or distributed queries without the need for osquery's tls plugin. sqhunter allows you to query open network sockets and check them against threat intelligence sources.
* [sysmon-config](https://github.com/SwiftOnSecurity/sysmon-config) - Sysmon configuration file template with default high-quality event tracing
* [sysmon-modular](https://github.com/olafhartong/sysmon-modular) - A repository of sysmon configuration modules
* [traceroute-circl](https://github.com/CIRCL/traceroute-circl) - Extended traceroute to support the activities of CSIRT (or CERT) operators. Usually CSIRT team have to handle incidents based on IP addresses received. Created by Computer Emergency Response Center Luxembourg.
* [X-Ray 2.0](https://www.raymond.cc/blog/xray/) - Windows utility (poorly maintained or no longer maintained) to submit virus samples to AV vendors.

## Playbooks

* [AWS Incident Response Runbook Samples](https://github.com/aws-samples/aws-incident-response-runbooks/tree/0d9a1c0f7ad68fb2c1b2d86be8914f2069492e21) - AWS IR Runbook Samples meant to be customized per each entity using them. The three samples are: "DoS or DDoS attack", "credential leakage", and "unintended access to an Amazon S3 bucket".
* [Counteractive Playbooks](https://github.com/counteractive/incident-response-plan-template/tree/master/playbooks) - Counteractive PLaybooks collection.
* [GuardSIght Playbook Battle Cards](https://github.com/guardsight/gsvsoc_cirt-playbook-battle-cards) - A collection of Cyber Incident Response Playbook Battle Cards
* [IRM](https://github.com/certsocietegenerale/IRM) - Incident Response Methodologies by CERT Societe Generale.
* [PagerDuty Incident Response Documentation](https://response.pagerduty.com/) - Documents that describe parts of the PagerDuty Incident Response process. It provides information not only on preparing for an incident, but also what to do during and after. Source is available on [GitHub](https://github.com/PagerDuty/incident-response-docs).
* [Phantom Community Playbooks](https://github.com/phantomcyber/playbooks) - Phantom Community Playbooks for Splunk but also customizable for other use.
* [ThreatHunter-Playbook](https://github.com/OTRF/ThreatHunter-Playbook) - Playbook to aid the development of techniques and hypothesis for hunting campaigns.

## Process Dump Tools

* [Microsoft ProcDump](https://docs.microsoft.com/en-us/sysinternals/downloads/procdump) - Dumps any running Win32 processes memory image on the fly.
* [PMDump](http://www.ntsecurity.nu/toolbox/pmdump/) - Tool that lets you dump the memory contents of a process to a file without stopping the process.

## Sandboxing/Reversing Tools

* [Any Run](https://app.any.run/) - Interactive online malware analysis service for dynamic and static research of most types of threats using any environment.
* [CAPA](https://github.com/mandiant/capa) - detects capabilities in executable files. You run it against a PE, ELF, .NET module, or shellcode file and it tells you what it thinks the program can do.
* [CAPEv2](https://github.com/kevoreilly/CAPEv2) - Malware Configuration And Payload Extraction.
* [Cuckoo](https://github.com/cuckoosandbox/cuckoo) - Open Source Highly configurable sandboxing tool.
* [Cuckoo-modified](https://github.com/spender-sandbox/cuckoo-modified) - Heavily modified Cuckoo fork developed by community.
* [Cuckoo-modified-api](https://github.com/keithjjones/cuckoo-modified-api) - Python library to control a cuckoo-modified sandbox.
* [Cutter](https://github.com/rizinorg/cutter) - Free and Open Source Reverse Engineering Platform powered by rizin.
* [Ghidra](https://github.com/NationalSecurityAgency/ghidra) - Software Reverse Engineering Framework.
* [Hybrid-Analysis](https://www.hybrid-analysis.com/) - Free powerful online sandbox by CrowdStrike.
* [Intezer](https://analyze.intezer.com/#/) - Intezer Analyze dives into Windows binaries to detect micro-code similarities to known threats, in order to provide accurate yet easy-to-understand results.
* [Joe Sandbox (Community)](https://www.joesandbox.com/) - Joe Sandbox detects and analyzes potential malicious files and URLs on Windows, Android, Mac OS, Linux, and iOS for suspicious activities; providing comprehensive and detailed analysis reports.
* [Mastiff](https://github.com/KoreLogicSecurity/mastiff) - Static analysis framework that automates the process of extracting key characteristics from a number of different file formats.
* [Metadefender Cloud](https://www.metadefender.com) - Free threat intelligence platform providing multiscanning, data sanitization and vulnerability assessment of files.
* [Radare2](https://github.com/radareorg/radare2) - Reverse engineering framework and command-line toolset.
* [Reverse.IT](https://www.reverse.it/) - Alternative domain for the Hybrid-Analysis tool provided by CrowdStrike.
* [Rizin](https://github.com/rizinorg/rizin) - UNIX-like reverse engineering framework and command-line toolset
* [StringSifter](https://github.com/fireeye/stringsifter) - A machine learning tool that ranks strings based on their relevance for malware analysis.
* [Threat.Zone](https://app.threat.zone) - Cloud based threat analysis platform which include sandbox, CDR and interactive analysis for researchers.
* [Valkyrie Comodo](https://valkyrie.comodo.com) - Valkyrie uses run-time behavior and hundreds of features from a file to perform analysis.
* [Viper](https://github.com/viper-framework/viper) - Python based binary analysis and management framework, that works well with Cuckoo and YARA.
* [Virustotal](https://www.virustotal.com) - Free online service that analyzes files and URLs enabling the identification of viruses, worms, trojans and other kinds of malicious content detected by antivirus engines and website scanners.
* [Visualize_Logs](https://github.com/keithjjones/visualize_logs) - Open source visualization library and command line tools for logs (Cuckoo, Procmon, more to come).
* [Yomi](https://yomi.yoroi.company) - Free MultiSandbox managed and hosted by Yoroi.

## Scanner Tools

* [Fenrir](https://github.com/Neo23x0/Fenrir) - Simple IOC scanner. It allows scanning any Linux/Unix/OSX system for IOCs in plain bash. Created by the creators of THOR and LOKI.
* [LOKI](https://github.com/Neo23x0/Loki) - Free IR scanner for scanning endpoint with yara rules and other indicators(IOCs).
* [Spyre](https://github.com/spyre-project/spyre) - Simple YARA-based IOC scanner written in Go

## Timeline Tools

* [Aurora Incident Response](https://github.com/cyb3rfox/Aurora-Incident-Response) - Platform developed to build easily a detailed timeline of an incident.
* [Highlighter](https://www.fireeye.com/services/freeware/highlighter.html) - Free Tool available from Fire/Mandiant that will depict log/text file that can highlight areas on the graphic, that corresponded to a key word or phrase. Good for time lining an infection and what was done post compromise.
* [Morgue](https://github.com/etsy/morgue) - PHP Web app by Etsy for managing postmortems.
* [Plaso](https://github.com/log2timeline/plaso) -  a Python-based backend engine for the tool log2timeline.
* [Timesketch](https://github.com/google/timesketch) - Open source tool for collaborative forensic timeline analysis.

## Videos

* [The Future of Incident Response](https://www.youtube.com/watch?v=bDcx4UNpKNc) - Presented by Bruce Schneier at OWASP AppSecUSA 2015.

## Windows Evidence Collection

* [AChoir](https://github.com/OMENScan/AChoir) - Framework/scripting tool to standardize and simplify the process of scripting live acquisition utilities for Windows.
* [Crowd Response](http://www.crowdstrike.com/community-tools/) - Lightweight Windows console application designed to aid in the gathering of system information for incident response and security engagements. It features numerous modules and output formats.
* [Cyber Triage](http://www.cybertriage.com) - Cyber Triage has a lightweight collection tool that is free to use. It collects source files (such as registry hives and event logs), but also parses them on the live host so that it can also collect the executables that the startup items, scheduled, tasks, etc. refer to. It's output is a JSON file that can be imported into the free version of Cyber Triage. Cyber Triage is made by Sleuth Kit Labs, which also makes Autopsy. 
* [DFIR ORC](https://dfir-orc.github.io/) - DFIR ORC is a collection of specialized tools dedicated to reliably parse and collect critical artifacts such as the MFT, registry hives or event logs. DFIR ORC collects data, but does not analyze it: it is not meant to triage machines. It provides a forensically relevant snapshot of machines running Microsoft Windows. The code can be found on [GitHub](https://github.com/DFIR-ORC/dfir-orc).
* [FastIR Collector](https://github.com/SekoiaLab/Fastir_Collector) - Tool that collects different artifacts on live Windows systems and records the results in csv files. With the analyses of these artifacts, an early compromise can be detected.
* [Fibratus](https://github.com/rabbitstack/fibratus) - Tool for exploration and tracing of the Windows kernel.
* [Hoarder](https://github.com/muteb/Hoarder) - Collecting the most valuable artifacts for forensics or incident response investigations.
* [IREC](https://binalyze.com/products/irec-free/) - All-in-one IR Evidence Collector which captures RAM Image, $MFT, EventLogs, WMI Scripts, Registry Hives, System Restore Points and much more. It is FREE, lightning fast and easy to use.
* [Invoke-LiveResponse](https://github.com/mgreen27/Invoke-LiveResponse) -  Invoke-LiveResponse is a live response tool for targeted collection.
* [IOC Finder](https://www.fireeye.com/services/freeware/ioc-finder.html) - Free tool from Mandiant for collecting host system data and reporting the presence of Indicators of Compromise (IOCs). Support for Windows only. No longer maintained. Only fully supported up to Windows 7 / Windows Server 2008 R2.
* [IRTriage](https://github.com/AJMartel/IRTriage) - Incident Response Triage - Windows Evidence Collection for Forensic Analysis.
* [KAPE](https://www.kroll.com/en/services/cyber-risk/incident-response-litigation-support/kroll-artifact-parser-extractor-kape) - Kroll Artifact Parser and Extractor (KAPE) by Eric Zimmerman. A triage tool that finds the most prevalent digital artifacts and then parses them quickly. Great and thorough when time is of the essence.
* [LOKI](https://github.com/Neo23x0/Loki) - Free IR scanner for scanning endpoint with yara rules and other indicators(IOCs).
* [MEERKAT](https://github.com/TonyPhipps/Meerkat) - PowerShell-based triage and threat hunting for Windows.
* [Panorama](https://github.com/AlmCo/Panorama) - Fast incident overview on live Windows systems.
* [PowerForensics](https://github.com/Invoke-IR/PowerForensics) - Live disk forensics platform, using PowerShell.
* [PSRecon](https://github.com/gfoss/PSRecon/) - PSRecon gathers data from a remote Windows host using PowerShell (v2 or later), organizes the data into folders, hashes all extracted data, hashes PowerShell and various system properties, and sends the data off to the security team. The data can be pushed to a share, sent over email, or retained locally.
* [RegRipper](https://github.com/keydet89/RegRipper3.0) - Open source tool, written in Perl, for extracting/parsing information (keys, values, data) from the Registry and presenting it for analysis.

## Resources 📖
- **Incident Response Process**: The incident response process consists of six stages: 
  1. **Preparation**: Establish response plans and tools.
  2. **Identification**: Detect incidents through monitoring and alerts.
  3. **Containment**: Isolate affected systems to prevent further damage.
  4. **Eradication**: Remove the root cause and any remnants of the attack.
  5. **Recovery**: Restore systems and data to a secure state.
  6. **Lessons Learned**: Document the incident and improve future response strategies.
- **[NIST Computer Security Incident Handling Guide](https://csrc.nist.gov/publications/detail/sp/800-61/rev-2/final)**: A comprehensive guide for incident response based on NIST standards.

## Useful Links 🌍
- **[SANS Incident Response](https://www.sans.org/incident-response/)**: A resource hub with articles, tools, and training materials focused on incident response.
- **[CISA Incident Response](https://www.cisa.gov/incident-response)**: The Cybersecurity and Infrastructure Security Agency (CISA) provides incident response resources and guidance.
