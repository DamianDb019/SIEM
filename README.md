<h1>Honey Pot Setup w/ Live Cyber Attacks</h1>


<h2>Description</h2>
Set up Azure Sentinel (SIEM) and connected it to a live VM (Honey Pot)
While I observed live RDP Brute Force attacks from around the world
<br />


<h2>Language Used</h2>

- <b>PowerShell</b> 

<h2>Environments Used </h2>

- <b>Azure</b> 
- <b>RDP</b>

<h2>Program walk-through:</h2>

<p align="center">
Created a VM in Azure: <br/>
<img src="https://i.imgur.com/9XzSOwO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create Log Analytics Workspace:  <br/>
<img src="https://i.imgur.com/LCl5Har.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enabled VM logs to be gathered in the Security Center: <br/>
<img src="https://i.imgur.com/OrZ9Acy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Connect Log Analytics to VM:  <br/>
<img src="https://i.imgur.com/6ZwypC5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Logged into the VM with RDP on my machine & Checked Event Viewer:  <br/>
<img src="https://i.imgur.com/rR4cBoP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Signed up and retrieved API Key from http://geolocation.io/:  <br/>
<img src="https://i.imgur.com/dKmTQFp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Input API key into Powershell Script and ran script:  <br/>
<img src="https://i.imgur.com/XEpyFHF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Created a custom table called Failed_RDP_WITH_GEO_CL:  <br/>
<img src="https://i.imgur.com/2Wy7IWx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
ChatGPT created me a KQL Query to extract raw custom log data:  <br/>
<img src="https://i.imgur.com/RxJDxAG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Set up a map in Microsoft Sentine:  <br/>
<img src="https://i.imgur.com/nQfVWGV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Reviewed MITRE Att&ck :  <br/>
<img src="https://i.imgur.com/7TBwluv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
