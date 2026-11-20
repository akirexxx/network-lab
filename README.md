# Windows Server & Ubuntu Infrastructure Lab

# Network & Infrastructure Lab

A hands-on infrastructure and cybersecurity lab built in VMware as part
of my IT security studies.

The project involved setting up and securing a virtual network
environment using Windows Server and Ubuntu Server, with a focus on
system administration, network configuration and security.

---

## 🖥️ Lab environment

| Component | Configuration |
|---|---|
| Virtualization | VMware |
| Windows server | Windows Server 2025 |
| Linux server | Ubuntu Server 26.04 |
| Domain | `nordkap.internal` |
| Network | NAT – `192.168.113.0/24` |

## 🛠️ Technologies & tools

| Windows | Linux | Networking & scripting |
|---|---|---|
| Active Directory | Apache | NAT |
| DNS | UFW | IP forwarding |
| Group Policy (GPO) | Linux permissions | Firewall rules |
| NTFS permissions | SMB / smbclient | Bash & PowerShell |
| Windows Firewall | Access logs | Regular expressions |

---

## What I built

### 1. Windows Server & Active Directory

-   Set up a domain controller with Active Directory and DNS.
-   Created users, organizational units (OUs) and security groups.
-   Configured shared folders with department-specific access
    permissions.
-   Applied Group Policy Objects (GPOs) for drive mapping and logon
    auditing.
-   Configured Windows Firewall to restrict incoming traffic and SMB
    access.

### 2. Ubuntu Server

-   Installed and configured Apache as a web server.
-   Created an internal webpage.
-   Configured Linux users, groups, ownership and file permissions.
-   Applied firewall rules using UFW.
-   Connected to Windows shared folders using `smbclient`.

### 3. Networking

-   Configured virtual network interfaces and static IP addresses in
    VMware.
-   Experimented with NAT and IP forwarding to provide internet access
    between virtual machines through Ubuntu.
-   Configured and tested firewall rules to control which machines could
    access specific services and ports.

### 4. Scripting & monitoring

-   **Bash:** Created a script using regular expressions to extract IP
    addresses and requested paths from Apache access logs, filtering for
    HTTP 404 responses.
-   **PowerShell:** Developed a script to monitor DNS and DHCP service
    status and automatically log the results using Windows Task
    Scheduler.

------------------------------------------------------------------------

## What I learned

Through this project, I gained practical experience in:

-   Managing a Windows domain environment using Active Directory and
    Group Policy.
-   Understanding authentication, authorization and access control.
-   Configuring network services, IP addressing, NAT and firewalls.
-   Working with Linux administration and file permissions.
-   Understanding communication and file sharing between Windows and
    Linux.
-   Using logs to identify potentially suspicious activity.
-   Automating administrative tasks using Bash and PowerShell.
-   Building and troubleshooting virtual environments in VMware.

------------------------------------------------------------------------

## Project structure

``` text
network-lab/
│
├── README.md
│
├── documentation/
    └── lab-report.pdf
```

## Author

Lotta Reiman

