<h1>Azure Storage Account</h1>

<h2>Description</h2>
This lab will configure an Azure Storage account.<br /><br />

Azure Storage Accounts provide a scalable and secure way to store and manage data in the cloud. They support various storage types, including:
<br /><br />

<b>Blob Storage:</b> For storing unstructured data like images, videos, and backups.
<br />
<b>File Storage:</b> Managed file shares accessible via SMB (Server Message Block) protocol.
<br />
<b>Queue Storage:</b> For storing and processing messages asynchronously between application components.
<br />
<b>Table Storage:</b> A NoSQL key-value store for structured data.
<br />
<b>Disk Storage:</b> Managed disks for Azure Virtual Machines.


<h2>Environments Used </h2>

- <b>Microsoft Azure</b>

<h2>Lab walk-through:</h2>

<p align="center">
<h4>Topology</h4>
Below, we have created a VN. This VN has 2 subnets. <br/>
We will configure an azure private dns service, so that resources in the VN can communicate using FQDNs.<br/>
<img src="https://i.imgur.com/EJ6N21j.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<h4>Step 1</h4> 
Create a Private DNS Zone.<br/>
<img src="https://i.imgur.com/hlsO0PS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h4>Step 2</h4> 
In your private DNS Zone. Link it to your VN.<br/>
<img src="https://i.imgur.com/TtmcQnQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/q5ap1Dy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/><br/>

Use auto registration to ensure that your VMs are automatically aded to the record sets.
<img src="https://i.imgur.com/2PEsAfV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<h4>Step 3</h4> 
After the setup is doen your VMs can communicate using FQDNs..<br/>
<img src="https://i.imgur.com/HkfDJ4W.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
