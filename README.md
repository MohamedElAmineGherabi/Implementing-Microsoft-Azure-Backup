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
Task 1: Creating a Resource Group <br/>
<br />
<br />
<img src="https://i.imgur.com/IuKZ9pg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/AvlV1ke.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/4qXpyAi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/zkzdioE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/xwjXv0o.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/2ieH3Oi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<p align="center">
Task 2: Setting Up a Virtual Network and Subnet <br/>
<br />
<br />
<img src="https://i.imgur.com/7J4tkMc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/aEQ0t9G.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/Xuk739S.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/E0R7zrJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/fCXz9Lp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/WiTvVJD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/nsTNNGF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/ovafc8O.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/kMlvsGX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/IyI1Obm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/EvJ5Zlt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
  
<p align="center">
Task 3: Securing the Subnet with a Network Security Group (NSG) <br/>
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
Task 4: Deploying Azure Bastion for Secure VM Access  <br/>
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
Task 5: Creating an Ubuntu Virtual Machine  <br/>
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
Task 6: Installing Nextcloud via SSH  <br/>
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
Task 7: Publishing the Web Server with a Public IP  <br/>
<br />
<br />
<img src="https://i.imgur.com/p83mVQU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/2S02Ajl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/DYOT32I.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/qmCTICr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/8p9rxJp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/UbAPifN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/xAvpgeF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/sJ9ZXeK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/1bqjGY7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/eknd9S4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/wWn7WEH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/HhLgtAQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />

<p align="center">
Task 8: Creating a DNS Label  <br/>
<br />
<br />
<img src="https://i.imgur.com/27QDWxp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/CXQ9GzX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/KYfnYwi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/TZqnu6I.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/mL8Mm7L.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/BCAOtl4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/7ip174O.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/WBdI9Vm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


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
