<h1>USB Forensic Investigation Lab</h1>



<h2>Description</h2>
This project documents a Windows USB forensic investigation in which I analyzed system artifacts to determine whether a USB storage device had been connected and used to access or transfer files. The investigation focused on collecting, analyzing, and correlating forensic evidence to reconstruct user activity and build a timeline of events.
<br />
<h2>Objectives</h2>

-<b>Identify connected USB storage devices.</b>

-<b>Determine when devices were first and last connected.</b>

-<b>Analyze user activity related to removable media.</b>

-<b>Correlate Windows artifacts to reconstruct a timeline.</b>

-<b>Document findings using industry-standard forensic methodology.</b>


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>FTK Imager</b>
- <b>USBDeview</b>
- <b>Autopsy</b>

<h2>Environments Used </h2>

- <b>Windows 11</b>

<p align="center">
To start my home lab scenario I Created Files For Investigation. Simulating confidential work files that would be found on a company computer: <br/>
<img src="screenshots forensics case/Screenshot 2026-05-10 095309.png"80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
I then Copied the Confidential files to a usb device(Usb device simulating a employee attemping to steal data from the company computer.:  <br/>
<img src="screenshots forensics case/Screenshot 2026-05-10 095939.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Using USBDeview I Gathered Vital information such as the devices name, serial number, first insert, last insert, last removal: <br/>
<img src="screenshots forensics case/Screenshot 2026-05-10 100230.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
By Clicking on the device in USBDeview i found a more detailed description of the usb deivce that was inserted into the computer. I Kept records of my findings for later use.  <br/>
<img src="screenshots forensics case/Screenshot 2026-05-10 100300.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Using FTK Imager I took a full image of the usb device(For time purposes use a small storage usb, the bigger the usb the longer the image will take). Taking Physical image of the device as it captures deleted files, unallocated space, and file system metadata which is typically used in a real world scenario(image format- E01-Expert witness format).:  <br/>
<img src="screenshots forensics case/Screenshot 2026-05-10 100832.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Keeping record of the image summary such as the hashes to ensure integrity of evidence. This was important as evidence can easily be tampered with so i want to make sure the hashes match.:  <br/>
<img src="screenshots forensics case/Screenshot 2026-05-10 102752.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <img src="screenshots forensics case/Screenshot 2026-05-10 112918.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Uploaded my image to autopsy for analysis, gathered information from the file system, metadata. Created a timeline reconstruction and recovered the deleted file( Employee deleted the file from the usb device to cover tracks):  <br/>
<img src="screenshots forensics case/Screenshot 2026-05-10 114217.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <img src="screenshots forensics case/Screenshot 2026-05-10 114706.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="screenshots forensics case/Screenshot 2026-05-10 115910.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
   <img src="screenshots forensics case/Screenshot 2026-05-10 115934.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 
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
