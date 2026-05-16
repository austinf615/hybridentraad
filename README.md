<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Configuring Hybrid Active Directory with Entra</h1>
This project outlines the implementation of a hybrid Active Directory environment using Azure virtual machines and Microsoft Entra Connect, enabling on-premises domain user accounts to synchronize with Microsoft Entra ID for cloud identity management.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Microsoft Entra Connect
- Remote Desktop
- Active Directory Domain Services
- Active Directory Users and Computers

<h2>Operating Systems Used </h2>

- Windows Server 2025 Datacenter

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1: Prepare the On-Premises Active Directory Environment
- Step 2: Install and Configure Microsoft Entra Connect Sync
- Step 3: Validate Hybrid Identify Synchronization and Functionality

<h2>Deployment and Configuration Steps</h2>

---

## Step 1: Prepare the On-Premises Active Directory Environment

---

<p>
<img width="1624" height="971" alt="AD-VM RD Info" src="https://github.com/user-attachments/assets/1f350b16-e963-4538-a9d3-3fe8ecf1f604" />
</p>
<p>
  
- Recorded the public IP address of the Domain-Controller virtual machine to establish a Remote Desktop connection for Active Directory administration.

</p>
<br />

<p>
<img width="1512" height="949" alt="AD-VM ADUC Nav" src="https://github.com/user-attachments/assets/613a0dd2-14ee-48d3-ba26-b6be8e1b08cf" />
</p>
<p>

- Connected to the domain controller using Remote Desktop with domain admin credentials and opened Active Directory Users and Computers (ADUC) to review the existing on-premises Active Directory environment.

</p>
<br />

<p>
<img width="1512" height="949" alt="AD-VM Users" src="https://github.com/user-attachments/assets/78d1edeb-51aa-4ca8-9843-e3d392e7e014" />
</p>
<p>

- Verified that existing domain user accounts were present in Active Directory, confirming that the on-premises identity environment was ready for synchronization with Microsoft Entra ID.

</p>
<br />

---

Step 2: Install and Configure Microsoft Entra Connect Sync

---

<p>
<img width="1624" height="971" alt="Entra Connect Download" src="https://github.com/user-attachments/assets/9c75eead-79f7-4d32-86a1-4793304a4ad4" />
</p>
<p>

- Accessed the Microsoft Entra Admin environment and downloaded Microsoft Entra Connect Sync onto the domain controller to begin configuring hybrid identity synchronization between on-premises Active Directory and Microsoft Entra ID.

</p>
<br />

<p>
<img width="1624" height="971" alt="Entra Setup1" src="https://github.com/user-attachments/assets/901bd0b1-4011-4c6c-afa3-3186070f918a" />
</p>
<p>

- Launched the Microsoft Entra Connect setup wizard and authenticated using Microsoft Entra Global Administrator credentials to connect the cloud identity tenant.

</p>
<br />

<p>
<img width="1624" height="971" alt="Entra Setup2" src="https://github.com/user-attachments/assets/20358fdb-cfa1-4549-998b-a650a661d091" />
</p>
<p>

- Provided on-premises Active Directory Domain Services (AD DS) administrative credentials to authorize synchronization between the local domain environment and Microsoft Entra ID.

</p>
<br />

<p>
<img width="1624" height="971" alt="Entra Setup End" src="https://github.com/user-attachments/assets/9e752001-47cb-4b1c-8f87-c6faef023113" />
</p>
<p>

- Successfully completed Microsoft Entra Connect configuration, enabling synchronization between the on-premises Active Directory environment and Microsoft Entra ID to support hybrid identity management.

</p>
<br />

---

Step 3: Validate Hybrid Identify Synchronization and Functionality

---

<p>
<img width="1624" height="971" alt="Entra Synced" src="https://github.com/user-attachments/assets/4f7a2814-3834-4341-abdb-7766de4ab321" />
</p>
<p>

- Verified that on-premises Active Directory user accounts successfully appeared in Microsoft Entra ID, confirming successful hybrid identity synchronization. This allows synchronized users to be managed across both environments and supports cloud-based identity services such as Microsoft 365 access, group management, and multifactor authentication.

</p>
<br />

---

## Skills Developed

### Hybrid Identity Management

Gained hands-on experience configuring a hybrid identity environment by integrating on-premises Active Directory with Microsoft Entra ID using Microsoft Entra Connect.

### Active Directory Administration

Worked within Active Directory Domain Services (AD DS) to verify domain users, manage the on-premises identity environment, and prepare the directory for cloud synchronization.

### Microsoft Entra Administration

Developed familiarity with the Microsoft Entra Admin Center for cloud identity management, user verification, and hybrid identity monitoring.

### Microsoft Entra Connect Configuration

Installed and configured Microsoft Entra Connect Sync to establish synchronization between on-premises Active Directory and Microsoft Entra ID.

### Identity Synchronization

Configured and validated synchronization of on-premises user identities to the cloud, demonstrating understanding of directory synchronization workflows.

### Identity and Access Management (IAM) Fundamentals

Developed practical experience with identity lifecycle concepts including user synchronization, centralized identity management, cloud authentication services, and hybrid access control.

### Administrative Authentication Workflows

Used both Microsoft Entra Global Administrator credentials and on-premises domain administrative credentials to securely configure identity synchronization between environments.

### Remote Server Administration

Used Remote Desktop Protocol (RDP) to remotely access and manage the Windows Server environment hosting Active Directory services.

### Cloud Infrastructure Familiarity

Worked within Microsoft Azure virtual machine environments to support identity infrastructure deployment and hybrid cloud integration.

### Validation and Troubleshooting

Verified successful synchronization by comparing on-premises Active Directory users with synchronized Microsoft Entra ID identities, confirming proper hybrid functionality.

### Technical Documentation

Documented hybrid identity configuration, synchronization workflows, and validation procedures using structured technical documentation and screenshots.
