# 1. Pentesting Report [pentest-report.pdf]

### Scope
This penetration test was conducted on three networks in order to provide your company with a comprehensive risk assessment. The three networks were selected to cover range of operational systems and include both internal and external networks.
To begin with, we conducted a test on the externally facing webservices located in the organization’s DMZ, hosted on an Ubuntu server running Apache and serving on ports 80 and 443. Secondly, we approached a SunOS server which allows for external access to the internal network through the OpenSSH service. Based on its network connection it was surmised that this server had dual network connectivity from within the DMZ to the internal LAN. Finally, the third attack that was based on access gained on the local LAN.

### Objectives
The objective of this penetration test is to represent an end-to-end attack on a conglomerate network comprised of three sub-networks. It illustrates how an attack originating from outside of the organization can lead to a full compromise of identity within the organization, along with access to the operation and configuration of external facing resources e.g., commercial websites. A combination of attacks on three different operating systems is used to gain a foothold on the wider network and highlights the need for the implementation of an in-depth defense strategy in order to prevent this type of attack.

# 2. Remcos Malware Report [remcos-malware-report.pdf]


### Malware Lab Setup
This malware lab setup is comprised of the VirtualBox Hypervisor running on an iMac host. The hypervisor is running two virtual machines, Windows 7 32-Bit and Ubuntu 16.04. The Ubuntu machine is acting as a bridging machine between the host computer’s network and the internal virtual network

### Windows
In order to simulate a typical user environment on the Windows infection machine, applications such as Microsoft Office, Skype etc. were installed. These programs exhibit known vulnerabilities which can be leveraged by malware. As soon as all required software and analysis tools were downloaded for the Windows machine, its NAT internet connection to the host’s network was cut. In order to place the malware on the windows machine WinSCP was used to transfer files from the Ubuntu machine. All antivirus software on the Windows machine was disabled. The Malwarebytes malware scanner was left on the machine to perform system scans without taking any disruptive remedial action. In order to evade detection by malware, it can be helpful to rename analysis tools such as the Procmon process monitor.

### Ubuntu
The Ubuntu machine is used both for static analysis of malware and for network traffic analysis. Linux has a large selection of useful and lightweight tools that can be used to analyse executables, some of which are listed in the table below. The machine was also used as a gateway for situations where the Windows malware needed access to the internet in order to execute successfully.

# 3. Sality Botnet Report [sality-botnet-report.pdf]

The objective of this report is to research the workings of a selected botnet. The Sality botnet has been highly active globabally in various iterations for close to two decades and continues to be a significant threat to the present day. The significance of this botnet will be examined in terms of its impact on an operational level and on a global organisational level. Analysis of online research papers, datasets, and pcap files will be used to ascertain the botnet’s workings from a software perspective. According to some malware threat maps, Sality is still one of the most pervasive botnets in terms of attack frequency. This report aims to investigate whether these map results are due to legacy mislabeling or whether Sality is still highly active.

Sality is noteworthy due to its persistence over time and its multifaceted mechanism of action. The central virus facilitated attack through a large selection of malware techniques, including file injection, polymorphic code, trojan downloaders and many more. Uses include sending spam, keylogging, data exfiltration, system manipulation and further infection of other systems. Of particular interest is the peer-to-peer (P2P) control system employed. In contrast to a central command-and-control server, Sality creates a botnet through creation of a network of equipotent peers, with no central server. The security implications of this will be examined and assessed. Sality can be found globally, with particular concentrations in Venezuela, Romania and India.
