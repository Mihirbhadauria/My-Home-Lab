# My-Home-Lab
This repo showcases my homelab and all the cool things I am working on it!

# Home Lab Public Documentation
Welcome!
The purpose of this document is to showcase parts of my home lab in a safe manner to others for fun and learning purposes

First step is ensuring I am able to store all my static IPs in a file of some sort so that I am agnostic to changes in modems as I had previously replaced my TPG provided modem (vx220 g2v) with a Telstra Smart Gen 2.

I am using Telstra Smart Gen 2 as the main modem and the TPG provided modem as an access point (AP) via ethernet backhaul.

I had made a rookie mistake as initially the TPG modem was my main and Smart Gen 2 was the AP, so certain settings like turning off DHCP for TPG Modem was not done due to forgetting that part along with using WAN port which would have caused conflicts.

Also noted that the WAN subnet is the same subnet used by my main modem. I am assuming that the WAN IP I will not assign as that can cause conflicts and drop outs.

I have now changed the subnet for infrastructure related stuff to 192.168.10.x

The ISP uses 192.168.0.x for their needs and just for ease of use and minimisation of conflicts I am moving to 192.168.10.x and to future proof myself the VLAN will have changes in 3rd octet i.e 192.168.20.x or 192.168.30.x which will be used for a range of purposes.


| Device         | IP Address     | MAC Address     | Purpose                          |
|----------------|----------------|------------------|----------------------------------|
| Raspberry Pi   | 192.168.0.2    | xx:xx:xx:xx:xx:xx | Old homelab → future DNS server |
| My PC          | 192.168.0.3    | xx:xx:xx:xx:xx:xx | My usual rig                     |
| AOOSTAR NAS    | 192.168.0.4    | xx:xx:xx:xx:xx:xx | Main home server                 |




