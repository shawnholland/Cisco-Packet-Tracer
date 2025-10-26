<h1>Simple Network with Inter-VLAN Routing</h1>


<h2>Description</h2>
This documentation outlines the step-by-step process I followed to replicate a simple network with inter-VLAN routing. The topology and configuration were adapted from an instructional lab, with the purpose of reinforcing my understanding of VLANs, routing, and network topology design.
<br />


<h2>Software and Utilities Used</h2>

- <b>Cisco IOS Command-Line Interface (CLI)</b> 
- <b>Cisco Packet Tracer</b>

<h2>Configuration Walkthrough:</h2>

<p align="center">
First I placed a 2911 router at the top, two 2960 switches below, and 4 PC's below that: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/1.png" height="80%" width="80%" alt="Step 1"/><br /><br/>
Then I selected the copper straight-through cable to connect all devices: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/2.png" height="80%" width="80%" alt="Step 2"/><br /><br/>
FastEthernet0: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/3.png" height="80%" width="80%" alt="Step 3"/><br /><br/>
Select the decive you want to connect the cable to and use the first availible FastEthernet: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/4.png" height="80%" width="80%" alt="Step 4"/><br /><br/>
After everything is connected it should look like this: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/5.png" height="80%" width="80%" alt="Step 5"/><br /><br/>
Select the Switch0 and open the CLI: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/6.png" height="80%" width="80%" alt="Step 6"/><br /><br/>
Use the commands "enable' and "conf t" to go from privileged EXEC mode to global configuration mode: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/7.png" height="80%" width="80%" alt="Step 7"/><br /><br/>
Set up VLAN 10 and name it, then exiting: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/8.png" height="80%" width="80%" alt="Step 8"/><br /><br/>
Set ports to use the VLAN: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/9.png" height="80%" width="80%" alt="Step 9"/><br /><br/>
Exit current mode, then do "write memory": <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/10.png" height="80%" width="80%" alt="Step 10"/><br /><br/>
Use "show vlan brief": <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/11.png" height="80%" width="80%" alt="Step 11"/><br /><br/>
Now we'll do the same for Switch1: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/12.png" height="80%" width="80%" alt="Step 12"/><br /><br/>
Creating vlan20 this time: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/13.png" height="80%" width="80%" alt="Step 13"/><br /><br/>
Navigate to Router0 CLI: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/14.png" height="80%" width="80%" alt="Step 14"/><br /><br/>
type "no" for the first prompt: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/15.png" height="80%" width="80%" alt="Step 15"/><br /><br/>
Set up the interface for vlan10, set the default IP and subnet mask, give it a description, and execute the "no shutdown" command: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/16.png" height="80%" width="80%" alt="Step 16"/><br /><br/>
Do the the same thing for the vlan20 interface: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/17.png" height="80%" width="80%" alt="Step 17"/><br /><br/>
Go to each PC's IP configuration menu and assign them IP addresses, subnet masks, and defualt gateways: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/18.png" height="80%" width="80%" alt="Step 18"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/19.png" height="80%" width="80%" alt="Step 19"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/20.png" height="80%" width="80%" alt="Step 20"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/21.png" height="80%" width="80%" alt="Step 21"/><br /><br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/22.png" height="80%" width="80%" alt="Step 22"/><br /><br/>
Select a PC0 and go to the command prompt: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/23.png" height="80%" width="80%" alt="Step 23"/><br /><br/>
Use the "ping" command to try and ping the other device in the same subnet: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/24.png" height="80%" width="80%" alt="Step 24"/><br /><br/>
Using the "ping" command again, try to ping a device from the other VLAN, the first ping will fail because it's populating the arp table: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/25.png" height="80%" width="80%" alt="Step 25"/><br /><br/>
I retried the same command and got no time outs the second time: <br/>
<img src="https://github.com/shawnholland/Cisco-Packet-Tracer/blob/7248932fb7d647c1b6b7ee7325ddec11bf5aac16/Screenshots/26.png" height="80%" width="80%" alt="Step 26"/><br /><br/>
Using the "show ip arp" command back in the router CLI you can see thee the populated arp table: <br/>
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
