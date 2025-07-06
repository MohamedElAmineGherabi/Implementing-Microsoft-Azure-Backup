# Implementing Microsoft Azure Backup


<h2>Project Details</h2>
This lab focused on building a secure and accessible web server infrastructure on Microsoft Azure. The hands-on project provided me with a structured environment to go through the complete lifecycle of deploying a virtual machine, securing network access, and hosting a web application (Nextcloud). It provided practical experience in cloud infrastructure provisioning, network security configuration, and remote server management using Azure-native tools.<br />
<br />

**Tasks Breakdown:**

**Task 1: Creating a Resource Group**

The lab began with the creation of a dedicated Azure Resource Group to logically organize and manage all related resources. This foundational step ensured that all components of the deployment were grouped for easier monitoring, billing, and lifecycle management.

**Task 2: Setting Up a Virtual Network and Subnet**

A custom Virtual Network (VNet) was created along with a subnet to define the IP address space and network segmentation. This step laid the groundwork for secure communication between Azure resources.

**Task 3: Securing the Subnet with a Network Security Group (NSG)**

A Network Security Group was deployed and associated with the subnet to enforce inbound and outbound traffic rules. This task emphasized the importance of perimeter security and demonstrated how to restrict access to only necessary ports and protocols.

**Task 4: Deploying Azure Bastion for Secure VM Access**

Azure Bastion was configured to enable secure, browser-based RDP/SSH access to the virtual machine without exposing it to the public internet. This task highlighted best practices in remote access security.

**Task 5: Creating an Ubuntu Virtual Machine**

An Ubuntu Server VM was provisioned within the secured subnet. This step involved selecting the appropriate image, size, authentication method, and associating the VM with the previously created NSG and VNet.

**Task 6: Installing Nextcloud via SSH**

Using Azure Bastion, an SSH session was initiated to the Ubuntu VM. Nextcloud, a self-hosted productivity platform, was installed and configured. This task provided hands-on experience with Linux server administration and web application deployment.

**Task 7: Publishing the Web Server with a Public IP**

A public IP address was assigned to the VM to make the Nextcloud instance accessible over the internet. This step involved configuring DNS and ensuring the NSG allowed HTTP/HTTPS traffic.

**Task 8: Creating a DNS Label**

To simplify access, a DNS label was created and associated with the public IP. This allowed users to reach the Nextcloud server using a friendly domain name instead of a raw IP address.

<br />

**Key Takeaways:**

This lab provided a comprehensive walkthrough of deploying a secure, internet-accessible web application on Azure. Key skills developed include:

- Provisioning and managing Azure infrastructure components
- Configuring virtual networks and subnets
- Implementing network security using NSGs
- Using Azure Bastion for secure remote access
- Installing and configuring web applications on Linux VMs
- Publishing services with public IPs and DNS labels

These skills are essential for cloud engineers, DevOps professionals, IT administrators, as well as Cybersecurity professionals working with Azure environments.
<br />


<h2>Softwares and Utilities Used</h2>

- <b>Microsoft Azure Portal: Used for provisioning and managing all cloud resources.</b>
- <b>Azure Bastion: Enabled secure, browser-based SSH access to the VM.</b>
- <b>Ubuntu Server: Operating system used for hosting the Nextcloud application.</b>
- <b>Nextcloud: Open-source web application installed on the VM for file sharing and collaboration.</b> 


  

<h2>Environments Used </h2>

- <b>Azure Cloud Environment: All tasks were performed within the Azure ecosystem, leveraging its native tools and services for infrastructure, networking, and security.

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
