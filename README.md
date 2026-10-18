NetExec (NXC) Cybersecurity Tutorial

Author: MD Asikur Siam

Tool Purpose

NetExec (NXC) is an open-source cybersecurity tool used to assess network services and enumerate systems. This project demonstrates NetExec's SMB features in an authorized virtualized Active Directory lab.

Installation Instructions

On a supported Debian-based Linux system, install NetExec using the appropriate package or installation method for your environment.

sudo apt update
sudo apt install netexec

Verify the installation:

nxc --version

View the main help menu:

nxc -h

View SMB-specific options:

nxc smb -h

Basic Usage Instructions

General SMB command format:

nxc smb TARGET -u USERNAME -p 'PASSWORD'

Common options:

smb — Selects the SMB protocol.

-u — Specifies the username.

-p — Specifies the password.

-H — Specifies an NTLM hash.

--local-auth — Uses local account authentication.

--shares — Lists accessible SMB shares.

Only use these commands on systems you own or are authorized to assess.

Lab Environment

The demonstration uses a virtualized lab containing a Windows Server domain controller and two Windows 10 Enterprise computers.

The tutorial covers NetExec installation, help commands, SMB authentication testing, share enumeration, and other features demonstrated in the lab.

Video Demonstration

Video URL: Add your published video link here.

Part I Handbook

The original handbook and documentation from Part I are available in the docs/ folder of this repository.

Screenshots and Example Files

Screenshots from the NetExec demonstration are available in the screenshots/ folder. Supporting example files used during the demonstration are included in the examples/ folder, if applicable.

Strengths and Limitations

Strengths

Supports multiple network protocols.

Provides useful enumeration and authentication-testing features.

Helps security professionals assess systems in authorized environments.

Limitations

Requires suitable network access and permissions.

Results depend on the system configuration and available credentials.

Some features may require additional dependencies or setup.

Improper use can disrupt systems or violate security policies.

References and Resources

NetExec GitHub: https://github.com/Pennyw0rth/NetExec

NetExec documentation: https://www.netexec.wiki/

NetExec releases: https://github.com/Pennyw0rth/NetExec/releases

Disclaimer

This project is for educational purposes. NetExec should only be used on systems you own or have explicit permission to test.
