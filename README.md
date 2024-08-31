# Packet Tracer - Cable a Simple Network

## Objectives
Today, I'm going to walk you through the basics of using Packet Tracer. We’ll create a simple network with two hosts, and you’ll see why choosing the right cable type is crucial for connecting PCs.

## Step 1: Creating a Network Diagram with Two PCs

First, let’s start by getting familiar with Packet Tracer. When you look at the bottom left-hand corner of the screen, you’ll see various icons representing different device categories, like Routers, Switches, or End Devices.

As I move my cursor over these device categories, notice how the name of each category pops up in a box centered between the rows of devices. To get started, I’ll select the **End Devices** category. Once I’ve done that, you’ll see the available options for that category appear right next to it.

Now, let’s begin:
1. I’ll select **End Devices** from the options on the bottom left.
2. Next, I’m going to drag and drop two generic PCs (PC-PT) onto the Logical Workspace.
3. With our PCs in place, I’ll select **Connections** from the bottom left-hand corner.
4. Now, I’ll choose a **Copper Straight-Through** cable type.
5. I’m going to click on the first host, PC0, and connect the cable to the **FastEthernet** port.
6. Then, I’ll click on the second host, PC1, and connect the other end of the cable to its **FastEthernet** port.
7. Uh-oh, I see red dots on the connections! That tells me I’ve used the wrong cable type. Let’s fix that by clicking the red X on the right-hand side to delete the Copper Straight-Through cable.
8. Moving my cursor to the cable, I click to delete it.
9. Let’s try a **Copper Cross-Over** cable this time.
10. I’ll connect one end of the new cable to the **FastEthernet** port on PC0.
11. Finally, I’ll connect the other end to the **FastEthernet** port on PC1. Look at those green dots! That means we’ve got the correct cable type.

<p align="center">
<img src="https://github.com/user-attachments/assets/a1f4845c-962c-4121-bda4-ec2808a04938" height="" width="100%" alt="100%" />
</p>

## Step 2: Configuring Host Names and IP Addresses on the PCs

Now that we’ve set up our physical connections, it’s time to configure the PCs.

1. I’m going to start with PC0 by clicking on it. This opens up the PC0 window.
2. From here, I’ll select the **Config** tab.
3. To keep things organized, I’m changing the PC Display Name to **PC-A**.
4. Next, I’ll select the **FastEthernet0** tab on the left.
5. Here, I’ll type in the IP address `192.168.1.1` and the subnet mask `255.255.255.0` in the IP Configuration section.
6. With that done, I’ll close the PC-A configuration window by clicking the X in the upper right-hand corner.
7. Now, I’m moving on to PC1, which I’ll click to open.
8. In the PC1 window, I’ll go to the **Config** tab again.
9. I’m renaming this one to **PC-B** for clarity.
10. Under the **FastEthernet0** tab, I’ll input the IP address `192.168.1.2` and subnet mask `255.255.255.0`.
11. To verify the connection, I’ll switch back to PC-A, click on the **Desktop** tab, and then open **Command Prompt**.
12. Here, I’ll type `ping 192.168.1.2`, which is the IP address of PC-B, to test the connectivity.

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

## Step 3: Connecting the Computers to a Switch

Let’s step it up a notch by adding a switch to the network.

1. I’ll begin by deleting the Copper Cross-Over cable, as we’ll be using a different type of connection.
2. Next, I’ll select **Switches** from the options in the bottom left-hand corner.
3. I’m going to drag and drop a **2960 switch** into the Logical Workspace.
4. Again, I’ll go to **Connections** and this time, I’ll pick a **Copper Straight-Through** cable type.
5. I’ll connect the first host, **PC-A**, by attaching one end of the cable to its **FastEthernet0** port.
6. Then, I’ll connect the other end to the switch, **Switch0**, specifically to the **FastEthernet0/1** port. After about a minute, two green dots should appear, indicating that we’re using the correct cable.
7. Now, I’ll take another **Copper Straight-Through** cable.
8. I’ll connect **PC-B** to **FastEthernet0**.
9. The other end of the cable will go into **Switch0**, this time using the **FastEthernet0/2** port.
10. To check that everything’s working, I’ll open **PC-B**, click the **Desktop** tab, and launch **Command Prompt**.
11. I’ll type `ping 192.168.1.1` to test the connection back to PC-A.
12. Finally, I’ll click the **Check Results** button at the bottom of the instruction window to verify that our network topology is correct.

<p align="center">
<img src="https://github.com/user-attachments/assets/2450f174-d340-490f-8947-269a6e9583f1" height="" width="" alt="" />
</p>
