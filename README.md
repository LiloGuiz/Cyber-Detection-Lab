# Enterprise Detection Lab: Week 1 Setup

  ## 1. Project Objective

  The primary objective of this project is to build a simulated enterprise network environment to
  understand, execute, and detect common cybersecurity attacks. This lab will serve as a practical
  portfolio piece demonstrating hands-on skills in network administration, threat simulation, and
  security monitoring.

  ## 2. Lab Architecture Overview

  (This is where your diagram will go. See Part 2 below.)

  ## 3. Virtualization Platform

  *   **Hypervisor:** Oracle VirtualBox version 7.0
  *   **Host OS:** Windows 11

  ## 4. Network Configuration

  To ensure a safe and isolated environment, all virtual machines are connected to a VirtualBox NAT
  Network. This allows the VMs to communicate with each other and access the internet for updates,
  while being firewalled from the host machine's primary network.

  *   **Network Name:** CyberLabNet
  *   **CIDR:** 10.0.2.0/24
  *   **DHCP Enabled:** Yes
  *   **Justification:** Using a NAT Network is a secure and efficient method for creating an
  isolated lab. It prevents any simulated attacks from affecting the host or home network, providing
   a contained sandbox for experimentation.

  ## 5. Virtual Machines Deployed

  ### Kali-Attacker
  *   **Operating System:** Kali Linux 2024.2
  *   **Purpose:** This VM will serve as the attack platform, utilizing its pre-installed security
  tools to perform reconnaissance and exploitation against the target environment.
  *   **IP Address:** 10.0.2.15 (Assigned via DHCP)
