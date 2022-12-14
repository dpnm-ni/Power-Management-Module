
Autonomous Energy-efficient VM consolidation:

High energy consumption, inefficient resource usage, and service level agreement (SLA) violations are major challenges for cloud data centers. So, the main goal of the autonomous VM consolidation module is to reduce energy consumption and SLA violation for cloud data centers. 

Major Objectives:

This mechanism comprises three parts: Host mode detection, VM selection, and VM consolidation.
The overloaded and underloaded hosts are detected in the host mode detection module. We used the Local Regression Robust (LRR) algorithm for overload detection and the threshold mechanism for underload detection.

The VM selection part detects the VMs from the overloaded and underloaded host and prepares a VM migration list. In our work, once the host is detected as overloaded, the next phase is to select some specific VMs from the host for migration. So, the selection process of VMs is based on the current workload statistics, such as RAM, CPU, and bandwidth usage. We used an efficient algorithm for VM selection from the overloaded host named Minimum Migration Time and Maximum CPU Utilization (MMTMU). MMTMU algorithm selects a VM that needs minimum migration time with maximum CPU utilization compared to the other VMs that reside in a host.

The last part is an RL-based agent for optimal consolidation of VMs while considering energy efficiency and service guarantees.

Some selected VMs with highly dynamic workload patterns from the Planet Lab workload traces have been used for the real-time workload.

Requirements:

Simulation of cloud data center is done using CloudSim simulator (version 3.0.3, 4.0)
IDE: Eclipse with the latest JAVA
Common Math Library

Usage: 

Install prerequisites and import module VM Consolidation for Power Management Mechanism Project
Import required libraries by including JARs files
Choose the LRR policy 
Choose VM selection policy as MMTMU and MMT
In case of comparison, use data centers with different configurations, such as by changing the number of hosts and VMs 

Reference:

Follow our recent paper for a better understanding "Abbas, Khizar, Jibum Hong, Nguyen Van Tu, Jae-Hyoung Yoo, and James Won-Ki Hong. "Autonomous DRL-based energy efficient VM consolidation for cloud data centers." Physical Communication 55 (2022): 101925."

