<h1>Simple Network with Inter-VLAN Routing</h1>


<h2>Description</h2>
This documentation outlines the step-by-step process I followed to replicate a simple network with inter-VLAN routing. The topology and configuration were adapted from an instructional lab, with the purpose of reinforcing my understanding of VLANs, routing, and network topology design.
<br />


<h2>Software and Utilities Used</h2>

- <b>Cisco IOS Command-Line Interface (CLI)</b> 
- <b>Cisco Packet Tracer</b>

<h2>Configuration Walkthrough:</h2>

<p align="center">
Launch the utility: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select the disk:  <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Launch the utility: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/1.png" height="80%" width="80%" alt="Step 1"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/2.png" height="80%" width="80%" alt="Step 2"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/3.png" height="80%" width="80%" alt="Step 3"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/4.png" height="80%" width="80%" alt="Step 4"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/5.png" height="80%" width="80%" alt="Step 5"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/6.png" height="80%" width="80%" alt="Step 6"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/7.png" height="80%" width="80%" alt="Step 7"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/8.png" height="80%" width="80%" alt="Step 8"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/9.png" height="80%" width="80%" alt="Step 9"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/10.png" height="80%" width="80%" alt="Step 10"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/11.png" height="80%" width="80%" alt="Step 11"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/12.png" height="80%" width="80%" alt="Step 12"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/13.png" height="80%" width="80%" alt="Step 13"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/14.png" height="80%" width="80%" alt="Step 14"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/15.png" height="80%" width="80%" alt="Step 15"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/16.png" height="80%" width="80%" alt="Step 16"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/17.png" height="80%" width="80%" alt="Step 17"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/18.png" height="80%" width="80%" alt="Step 18"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/19.png" height="80%" width="80%" alt="Step 19"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/20.png" height="80%" width="80%" alt="Step 20"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/21.png" height="80%" width="80%" alt="Step 21"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/22.png" height="80%" width="80%" alt="Step 22"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/23.png" height="80%" width="80%" alt="Step 23"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/24.png" height="80%" width="80%" alt="Step 24"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/25.png" height="80%" width="80%" alt="Step 25"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/26.png" height="80%" width="80%" alt="Step 26"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/27.png" height="80%" width="80%" alt="Step 27"/><br /><br/>

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
