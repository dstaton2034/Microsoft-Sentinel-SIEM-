<h1>Microsoft Sentinel (SIEM)</h1>

 
<h2>Description</h2>
Discover the power of Microsoft Sentinel with this step-by-step guide showcasing my work. I successfully set up Microsoft Sentinel as a Security Information and Event Management (SIEM) system and connected it to a live virtual machine that acted as a honeypot. Real-time attacks, including RDP Brute Force, were observed from various parts of the world. A custom PowerShell script was utilized to identify the attacker's geolocation information and I was able to visualize it on the Azure Sentinel map through detailed screenshots
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 

<h2>Environments Used </h2>

- <b>Microsoft Sentinel</b>

<h2>Project walk-through:</h2>

<p align="center">
Setting up a VM in Azure: <br/>
<img src="https://i.imgur.com/bHQOsdB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Created my firewall rules to accept all traffic:  <br/>
<img src="https://i.imgur.com/qSiAhXA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Created a Log Analytics workspace: <br/>
<img src="https://i.imgur.com/8OYYfcI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 Connected Log Analytics to my VM (NO PICTURE)
 <br />
 <br />
Setting up Sentinel, connecting my VM I previously made to it:  <br/>
<img src="https://i.imgur.com/hdGiEbI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Connected to my VM through Remote Desktop:  <br/>
<img src="https://i.imgur.com/ZMp9VmB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Pinging my vm to make sure traffic can come through:  <br/>
<img src="https://i.imgur.com/GkZRWJX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Running a Powershell Strip (It just basically gets all the EventLog-SecurityLog grabs all the events of all the failed logins and creates a new logfile):  <br/>
<img src="https://i.imgur.com/7xotPhX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
Log that was created after running the strip:  <br/>
<img src="https://i.imgur.com/bWbro4o.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Creating a logfile to train log analytics what to look for in the logfile:  <br/>
<img src="https://i.imgur.com/O10T49w.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Making sure my logs came through successfully:  <br/>
<img src="https://i.imgur.com/1scymYy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Setting Up World MAP:  <br/>
<img src="https://i.imgur.com/rldHc8K.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Checking my powershell strip, noticed that people have discovered my VM and are trying to brute force
<img src="https://i.imgur.com/nyNNVZr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/RoodEet.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 
 
 
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
