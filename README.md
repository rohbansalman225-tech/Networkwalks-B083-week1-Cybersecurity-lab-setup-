Cybersecurity Lab Setup – VirtualBox & Kali Linux

📌 Project Overview

This project demonstrates the setup of a basic Cybersecurity Testing Lab Environment using Oracle VirtualBox and Kali Linux.

The lab was configured to provide a safe virtual environment for cybersecurity and ethical hacking practice.

🛠️ Technologies Used
Oracle VirtualBox
Kali Linux
NAT Network
7-Zip
Virtual Machine Snapshots

🎯 Tasks Completed
1. Install Required Software
Downloaded and installed 7-Zip
Downloaded and installed Oracle VirtualBox
Downloaded the Kali Linux Virtual Machine
2. Configure NAT Network

A custom NAT Network was created in VirtualBox with the following configuration:

Network Address: 10.0.0.0/24
Network Type: NATNetwork
Kali Linux IP Address: 10.0.0.2/24

This configuration allows virtual machines in the lab environment to communicate through the same virtual network.

3. Import Kali Linux

The Kali Linux virtual machine was imported into Oracle VirtualBox and configured as the main attacking/hacker machine for the cybersecurity lab.

4. Configure Kali Linux Network

The network adapter for Kali Linux was configured to use:

Attached To: NAT Network
Network Name: NATNetwork
IP Address: 10.0.0.2/24
Internet Access: Enabled
5. Enable Clipboard and Drag & Drop

The following VirtualBox features were enabled to improve interaction between the host machine and Kali Linux:

Shared Clipboard: Bidirectional
Drag and Drop: Bidirectional
6. Configure Shared Folder

A shared folder was configured between the host machine and Kali Linux.

Shared Folder: /downloads

This allows files to be shared between the host operating system and the virtual machine.

7. Create Virtual Machine Snapshot

After completing the configuration, a snapshot of the Kali Linux virtual machine was created.

This snapshot can be used to restore the lab environment if any configuration issues occur during future cybersecurity practice.

🌐 Network Configuration
Device	Network	IP Address
Kali Linux	NATNetwork	10.0.0.2/24

Network Range: 10.0.0.0/24

🚀 Future Lab Expansion

The lab can be expanded in the future by adding additional virtual machines such as:

Windows 10
Windows 11
Windows 7
Windows Server
Android

These machines can be connected to the same NAT Network for cybersecurity testing, penetration testing practice, and communication testing.

If Kali Linux does not have internet access:

Check that the NATNetwork was created correctly.
Verify the network adapter settings.
Make sure no other virtual machine is using 10.0.0.2.
Restart Kali Linux and VirtualBox.

The lab instructions also provide the following commands for certain VirtualBox and Kali Linux internet connectivity issues:

sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0
sudo nmcli connection down "Wired connection 1"
sudo nmcli connection up "Wired connection 1"
📚 Purpose

The purpose of this project is to create a safe and isolated environment for learning and practicing:

Cybersecurity
Ethical Hacking
Linux
Network Security
Penetration Testing
Virtualization
👨‍💻 Author

Rohban Salman

📌 Project Information
Program Name: Cybersecurity at Networkwalks | Week: 01 | Project: Cybersecurity and Pentesting Lab Setup | Repository: GitHub
Note: This lab setup is intended for educational and authorized cybersecurity practice only.
