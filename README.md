SDN Mininet Ryu Project

Description
This project demonstrates Software Defined Networking (SDN) using Mininet and the POX controller. It includes bandwidth analysis using iperf.

Topology
- 1 Switch (s1)
- 3 Hosts (h1, h2, h3)

Technologies Used
- Mininet
- POX Controller
- OpenFlow
- Python

Steps to Run:-

Step 1. Start POX Controller
cd ~/pox
python3 pox.py forwarding.l2_learning

Step 2: Start Mininet
sudo mn --topo single,3 --controller=remote

Step 3: Test Connectivity
pingall

Step 4: Measure Bandwidth
iperf h1 h2


Output
- All hosts can communicate successfully (0% packet loss)
- Bandwidth is measured between hosts using iperf

Files Included
- controller.py
- setup.jpg
- flow.jpg
- iperf broadcast.jpg

Concepts Covered
- Software Defined Networking (SDN)
- OpenFlow protocol
- Network virtualization
- Traffic control
- Bandwidth measurement

