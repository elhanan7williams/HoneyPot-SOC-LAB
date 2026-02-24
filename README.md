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
Launch the utility: <br/>
<img src="https://image2url.com/r2/default/images/1771948988086-cde7d458-345d-4874-8e9c-26a8575287a9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
![image alt](https://github.com/elhanan7williams/HoneyPot-SOC-LAB/blob/main/Screenshot%202026-02-12%20155311.png?raw=true)

<br />
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
