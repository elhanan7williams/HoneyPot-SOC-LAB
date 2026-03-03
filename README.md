# HoneyPot-SOC-LAB
I deployed a Windows VM in Microsoft Azure as a honeypot to capture real attack attempts. I collected and analyzed failed login logs using KQL and visualized attacker locations with Microsoft Sentinel. This project improved my cloud security and threat detection skills.
<h2>Description</h2>
# Honeypot-Soc-Lab
I built a Windows honeypot in Microsoft Azure and exposed it to the internet to capture real attack activity. Logs were sent to Microsoft Sentinel, analyzed with KQL, enriched with GeoIP data, and visualized on an attack map to practice real SOC analyst workflows.




My project consisted of deploying a Windows virtual machine in Microsoft Azure and configuring it as a honeypot by allowing open inbound traffic and disabling the firewall. I generated failed login attempts and captured real-world brute-force activity from the internet. I set up a Log Analytics Workspace and connected Microsoft Sentinel as a SIEM to centralize and monitor security logs. Using the Azure Monitor Agent and Data Collection Rules, I forwarded Windows Security Events (such as Event ID 4625). I then used Kusto Query Language (KQL) to analyze attack data, enriched logs with geographic IP information using a Sentinel watchlist, and created an interactive attack map to visualize where login attempts were coming from globally


<h2>Languages and Utilities Used</h2>

- <b>Virtual Mchine(Windows 10)</b> 
- <b>Microsoft Sentinel</b>
- <b> Log Analytics</b>
- <b> Kusto Query Language</b>
- <b> Azure Monitor Agent</b>
- <b> Data Collection Rules</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">
Create Resource Group: <br/>
<img src="IMAGES/Screenshot 2026-02-12 155311.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<br />
Create Virtual Network (VNet):  <br/>
<img src="IMAGES/Screenshot 2026-02-12 155620.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Deploy Windows 10 Virtual Machine: <br/>
<img src="IMAGES/Screenshot 2026-02-12 161733.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Configure Network Security Group (Open RDP 3389):  <br/>
<img src="IMAGES/Screenshot 2026-02-12 163029.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Disable / Modify Local Firewall (Intentional Exposure):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create Log Analytics Workspace:  <br/>
<img src="IMAGES/Screenshot 2026-02-13 045514.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Install Azure Monitor Agent and Configure Data Collection Rules:  <br/>
<img src="IMAGES/Screenshot 2026-02-13 050336.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Analyze Captured Attack Logs:  <br/>
<img src="IMAGES/Screenshot 2026-02-13 103054.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Upload GeoIP On Watchlist:  <br/>
<img src="IMAGES/Screenshot 2026-02-13 103154.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Map Attacks To GeoIP:  <br/>
<img src="IMAGES/Screenshot 2026-02-13 105023.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Windows VM Attack Map:  <br/>
<img src="IMAGES/Screenshot 2026-02-13 105635.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
