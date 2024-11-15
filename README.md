# **VIRT-LAB: Oracle VirtualBox with Ubuntu & Kali**

## Objective

The goal of this project is to set up a virtualized environment using VirtualBox, install Ubuntu and Kali Linux, and update both systems to their latest versions.

### Skills Learned

- Installing Virtualization Software.
- Setting Up Virtual Machines.
- Operating System Installation.
- VirtualBox Network Configuration.
- Updating and Managing OS.

### Tools Used

- VirtualBox.
- Ubuntu.
- Kali Linux.

## Steps

1. **Download and Install VirtualBox** 📥💻

- Go to the VirtualBox website and download the Windows version of the program.
  
![1](https://github.com/user-attachments/assets/82100c74-dcfe-4f05-937a-97c53c693e54)

- Install VirtualBox on your system following the standard installation procedure.

 ![1 5](https://github.com/user-attachments/assets/a2f00376-c6d3-48e3-b1e4-dfd936683cf8)


2. **Download Ubuntu** 🌐🐧

- Visit the Ubuntu website and download the latest stable version of Ubuntu Desktop.

  ![2](https://github.com/user-attachments/assets/8113a50f-20c2-42d5-a706-c01005779593)
  ![2 5](https://github.com/user-attachments/assets/2ecc328e-0d85-4d8a-adfb-e7ad45c00f26)


3. **Download Kali Linux** 🌐💻🐍

- Go to the Kali Linux website and download the 64-bit ISO installer for Kali Linux.
  
![3](https://github.com/user-attachments/assets/9c359a6c-dd0d-4f55-8011-6f93869dc862)
![3 5](https://github.com/user-attachments/assets/97267f35-5da8-4f95-a67c-a0fec3d7fdb7)


4. **Set Up Virtual Machines in VirtualBox** 🛠️⚙️

- Open VirtualBox and click on the "New" button to create a new virtual machine.
- Follow the prompts to create a new VM for each operating system (Ubuntu and Kali Linux).

![4](https://github.com/user-attachments/assets/a11524ef-1a55-4ed8-9e6c-aaa99c0273de)

   4.1. **Configure the Ubuntu Virtual Machine** 🖥️⚙️

   - Name the first VM "Ubuntu" and select the previously downloaded Ubuntu ISO.
   - Configure the virtual machine settings.
   - Start the machine and follow the on-screen installation prompts to install Ubuntu.
   - Once installation is complete, reboot the VM.

![4 A](https://github.com/user-attachments/assets/3fe9c022-9c30-494f-838b-59c7d8ca8609)

   4.2. **Configure the Kali Linux Virtual Machine** 🖥️⚙️

   - Repeat the process to create the second virtual machine, name it "Kali", and select the Kali Linux ISO.
   - Install Kali Linux and complete the setup. Reboot the VM after installation.

![4 B](https://github.com/user-attachments/assets/3b244bfd-de2f-423b-9c38-96494a609f86)


5. **Verify Virtual Machines** ✅🖥️

- Ensure that both Ubuntu and Kali Linux VMs are successfully installed and booting properly in VirtualBox.

  ![5](https://github.com/user-attachments/assets/5274f22f-fee7-4b10-9a6f-3311693fbfaf)


### **Setting Up the Networking for VMs**

6. **Create a NAT Network in VirtualBox** 🌐🛠️

- In VirtualBox, go to File > Tools > Network Manager.
- In the Network Manager window, click the NAT Networks tab and click Create. This will automatically create a NAT network for your VMs.

![6](https://github.com/user-attachments/assets/c98885d7-1222-4de9-876b-3a5a35204062)
![6 1](https://github.com/user-attachments/assets/b257aefd-456e-4c52-a73e-062016898f73)


7. **Configure the Network Adapter for Ubuntu (NAT Network)** 🌐🔧🐧

- In VirtualBox, select the Ubuntu VM and click Settings.
- Under Network, enable the Network Adapter and set it to NAT Network.
- Choose the NAT network you just created and click OK.

![7](https://github.com/user-attachments/assets/888ba204-22f2-43d0-af6e-69c368dd6859)


8. **Configure the Network Adapter for Kali Linux (NAT Network)** 🌐🔧💻

- Repeat the same process from above for Kali Linux by selecting the Kali VM, going to Settings > Network, and configuring it to use the same NAT Network.

![8](https://github.com/user-attachments/assets/32ce623a-eb78-4626-a863-d2c8df3a5dca)


### **Updating the Operating Systems**

9. **Update Ubuntu** 🔄🐧

- Start the Ubuntu VM and open a terminal.
- Run the following commands to update the system and install essential tools:

    **sudo apt update && sudo apt upgrade -y**

  ![9](https://github.com/user-attachments/assets/6994f5e4-e216-41aa-84d2-bfc7bec43178)

    **sudo apt install -y build-essential git curl wget**

  ![9 5](https://github.com/user-attachments/assets/9c9f837f-3cb4-4528-bfcb-3612ad973b6f)

These commands will update the Ubuntu system and install essential utilities.


10. **Update Kali Linux** 🔄💻🐍

- Start the Kali Linux VM and open a terminal.
- Run the following commands to update the system and install security tools.

     **sudo apt update && sudo apt upgrade -y**

  ![10](https://github.com/user-attachments/assets/e368ffaf-23b5-474b-be64-6300dcbeaee4)

     **sudo apt install -y nmap wireshark metasploit-framework**

  ![10 5](https://github.com/user-attachments/assets/60a129ae-a9eb-4123-807a-022df1e98c71)


11. **Verify Updates** ✅🔍

Ensure both Ubuntu and Kali Linux systems are up-to-date and ready for use.


## Conclusion 🎉

In this project, we’ve successfully set up a VirtualBox lab with Ubuntu and Kali Linux to create an isolated testing environment for network simulations and penetration testing. We’ve configured network settings, updated both systems, and ensured everything is running smoothly. This foundational lab can now be used for further security research, testing, and simulation of attacks and defenses.






