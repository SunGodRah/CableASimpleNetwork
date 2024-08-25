# Packet Tracer - Cable a Simple Network

## Objectives
- Develop an understanding of the basic functions of Packet Tracer.
- Create a simple network with two hosts.
- Observe the importance of using the correct cable type to connect PCs.

## Step 1: Create a Network Diagram with Two PCs

The bottom left-hand corner of the Packet Tracer screen displays icons that represent device categories or groups, such as Routers, Switches, or End Devices.

Move your cursor over the device categories to show the name of the category in the box centered between the rows of devices. To select a device, first select the device category. Once the device category is selected, the options within that category appear in the box next to the category listings. Select the device option that is required.

1. Select **End Devices** from the options in the bottom left-hand corner.
2. Drag and drop two generic PCs (PC-PT) onto the Logical Workspace.
3. Select **Connections** from the bottom left-hand corner.
4. Choose a **Copper Straight-Through** cable type.
5. Click the first host, PC0, and assign the cable to the **FastEthernet** connector.
6. Click the second host, PC1, and assign the cable to the **FastEthernet** connector.
7. The red dots indicate an incorrect cable type. Click the red X on the right-hand side of Packet Tracer. This will allow you to delete the Copper Straight-Through cable.
8. Move the cursor to the cable and click the cable to delete it.
9. Choose a **Copper Cross-Over** cable type.
10. Click the first host, PC0, and assign the cable to the **FastEthernet** connector.
11. Click the second host, PC1, and assign the cable to the **FastEthernet** connector. The green dots at both ends of the cable indicate the correct cable type.

<p align="center">
<img src="https://github.com/user-attachments/assets/a1f4845c-962c-4121-bda4-ec2808a04938" height="" width="100%" alt="100%" />
</p>

## Step 2: Configure Host Names and IP Addresses on the PCs

1. Click PC0. A PC0 window will appear.
2. From the PC0 window, select the **Config** tab.
3. Change the PC Display Name to **PC-A**.
4. Select the **FastEthernet0** tab on the left.
5. Type the IP address `192.168.1.1` and subnet mask `255.255.255.0` in the IP Configuration section.
6. Close the PC-A configuration window by selecting the X in the upper right-hand corner.
7. Click PC1. A PC1 window will open.
8. From the PC1 window, select the **Config** tab.
9. Change the PC Display Name to **PC-B**.
10. Select the **FastEthernet0** tab on the left.
11. Type the IP address `192.168.1.2` and subnet mask `255.255.255.0` in the IP Configuration section.
12. Click PC-A and then click the **Desktop** tab.
13. Click **Command Prompt**.
14. Type `ping 192.168.1.2`. This is the address of the other computer.
15. Close the PC-B configuration window by selecting the X in the upper right-hand corner.

<p align="center">
<img src="https://github.com/user-attachments/assets/ae02f8d4-ea45-48be-851d-7245bf4ad9ae" height="100%" width="100%" alt="" />
</p>

<p align="center">
<img src="https://github.com/user-attachments/assets/5183eca4-4b96-4933-b1d3-480100b79748" height="100%" width="100%" alt="" />
</p>

<p align="center">
<img src="https://github.com/user-attachments/assets/56b9a0a1-2ff8-4dcd-8a92-687b5ac94280" height="100%" width="100%" alt="" />
</p>

<p align="center">
<img src="https://github.com/user-attachments/assets/fc2feaca-f834-49cd-b964-4a80fa7149e8" height="100%" width="100%" alt="" />
</p>

## Step 3: Connect the Computers to a Switch

1. Delete the Copper Cross-Over cable.
2. Select **Switches** from the options in the bottom left-hand corner.
3. Drag and drop a **2960 switch** onto the Logical Workspace.
4. Select **Connections** from the bottom left-hand corner.
5. Choose a **Copper Straight-Through** cable type.
6. Click the first host, **PC-A**, and assign the cable to the **FastEthernet0** connector.
7. Click the switch, **Switch0**, and select a connection port, **FastEthernet0/1**, to connect to PC-A. After about one minute, two green dots should appear on both sides of the Copper Straight-Through cable. This indicates the correct cable type has been used.
8. Click the Copper Straight-Through cable type again.
9. Click the second host, **PC-B**, and assign the cable to the **FastEthernet0** connector.
10. Click the switch, **Switch0**, and click **FastEthernet0/2** to connect to PC-B.
11. Click PC-B and then click the **Desktop** tab.
12. Click **Command Prompt**.
13. Type `ping 192.168.1.1`. This is the address of the other computer.
14. Click the **Check Results** button at the bottom of this instruction window to verify that the topology is correct.

<p align="center">
<img src="https://github.com/user-attachments/assets/2450f174-d340-490f-8947-269a6e9583f1" height="" width="" alt="" />
</p>
