# Implementing Microsoft Azure Backup


<h2>Project Details</h2>
This lab focused on implementing a full virtual machine backup solution using Microsoft Azure. The hands-on project provided me with a structured environment to explore Azure Backup capabilities, from setting up a Recovery Services Vault to configuring backup policies and protecting a virtual machine. It offered practical experience in cloud-based data protection and disaster recovery planning using Azure-native tools.<br />
<br />

**Tasks Breakdown:**

**Task 1: Creating a Recovery Services Vault**

A Recovery Services Vault was created to securely store backup data. This vault acts as a centralized management interface for all backup and recovery operations in Azure.

**Task 2: Configuring Backup Policies**

Backup policies were defined to automate the backup process. This included setting the frequency and retention period for daily backups, ensuring consistent protection of virtual machines.

**Task 3: Exercise: Creating a Monthly Backup Policy**

An exercise involved configuring a monthly backup policy to extend retention and support long-term data protection strategies.

**Task 4: Creating an Azure Virtual Machine**

A virtual machine was provisioned using the Free tier. This VM served as the target for backup operations and simulated a real-world workload environment.

**Task 5: Implementing Azure VM Backup**

The VM was registered with the Recovery Services Vault, and the backup policy was applied. A backup job was initiated to validate the configuration and ensure successful data protection.

**Task 6: Exercise: Creating a New VM with Monthly Backup**

An additional VM was created and protected using the monthly backup policy, demonstrating how to scale backup strategies across multiple resources.

<br />

**Key Takeaways:**

This lab provided a comprehensive walkthrough of Azure Backup for virtual machines. Key skills developed include:

- Creating and managing Recovery Services Vaults
- Defining and applying backup policies
- Automating VM backups in Azure
- Understanding retention strategies for daily and monthly backups
- Implementing cloud-native disaster recovery solutions

These skills are essential for cloud administrators, IT professionals, and cybersecurity practitioners responsible for data protection and business continuity in cloud environments.
<br />


<h2>Softwares and Utilities Used</h2>

- <b>Microsoft Azure Portal: Used for provisioning and managing all backup-related resources.</b>
- <b>Recovery Services Vault: Centralized service for managing backups.</b>
- <b>Azure Virtual Machines: Target resources for backup operations.</b>

  

<h2>Environments Used </h2>

- <b>Azure Cloud Environment: All tasks were performed within the Azure ecosystem, leveraging its native tools and services for backup, storage, and virtual machine management.

</b>

<h2>Program walk-through:</h2>




<p align="center">
Task 1: Creating a Recovery Services Vault <br/>
<br />
<br />
<img src="https://i.imgur.com/wetXW0q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/PVqr5e8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/M6pL5xX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/cKXiWVJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/DhSLeMr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/1G3wblQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<p align="center">
Task 2: Configuring Backup Policies <br/>
<br />
<br />
<img src="https://i.imgur.com/8v2noHz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/GWchhuc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/NRvxw0z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/VZqkaRl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/BHTy0IN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/b4G38E8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/IpyG3dC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/2jmX3nJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
  
<p align="center">
Task 3: Exercise: Creating a Monthly Backup Policy <br/>
<br />
<br />
<img src="https://i.imgur.com/Wnm1bmq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/PPMtGVt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/IUR7lM7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/Fa3Y9eV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/Sb5AlOf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/WjYkqIG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/N1TBLNX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/vXWFHMh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>




<br />
<br />
<br />
Task 4: Creating an Azure Virtual Machine  <br/>
<br />
<img src="https://i.imgur.com/kv4dHW1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/mfjzKU8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/TtrNXu2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/OgmZTQz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/M4pBsT9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/2IM1WFz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/uW5iG99.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />


<br />
<br />
Task 5: Implementing Azure VM Backup  <br/>
<br />
<img src="https://i.imgur.com/i4J3eyB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/OCAuLa5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/4LWeolG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/O84jObP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/FTjUGvM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/Eehp1dj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/QjYP3Lx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/W9GQWSa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />
<br />
<br />
Task 6: Exercise: Creating a New VM with Monthly Backup  <br/>
<br />
<img src="https://i.imgur.com/1ATP4VS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/WYqmJtZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/mMW1xd4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/Owdv1uY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/mQcyZHz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/G2CgPRt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br />
<img src="https://i.imgur.com/IuffyDQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<br />
<br />
<br />
<br />
<br />
<br />
<br />
<img src="https://i.imgur.com/LbRONpE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />










<br />
<br />

</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
