<h1>USB Forensic Investigation Lab</h1>



<h2>Description</h2>
This project documents a Windows USB forensic investigation in which I analyzed system artifacts to determine whether a USB storage device had been connected and used to access or transfer files. The investigation focused on collecting, analyzing, and correlating forensic evidence to reconstruct user activity and build a timeline of events.
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>FTK Imager</b>
- <b>USBDeview</b>
- <b>Autopsy</b>

<h2>Environments Used </h2>

- <b>Windows 11</b>

<p align="center">
Create Files For Investigation: <br/>
<img src="screenshots forensics case/Screenshot 2026-05-10 095309.png"80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Copy Confidential files to a usb device:  <br/>
<img src="screenshots forensics case/Screenshot 2026-05-10 095939.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Using USBDeview Gather Vital information such as the devices name, serial number, first insert, last insert, last removal: <br/>
<img src="screenshots forensics case/Screenshot 2026-05-10 100230.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Clicking on the device in USBDeview shows a more detailed description of said device that you can record for your investigation:  <br/>
<img src="screenshots forensics case/Screenshot 2026-05-10 100300.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
