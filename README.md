# 🏦 Multi-City Banking Enterprise Network Architecture

 A robust enterprise network simulation developed for a banking institution using Cisco Packet Tracer.  Built as a networking project for Air University, Islamabad, this architecture features a central corporate headquarters, dynamically routed branch communications, and rigorous ICMP connectivity validation.

---

## 🏢 Architecture Features

* **Geographic Distribution**: Simulates a network spanning 2 cities: Islamabad and Rawalpindi.
*  **Regional Branches**: Each city contains 3 independent branches.  Each branch is fully equipped with Personnel Working PCs, localized Servers, and inter-connected routers.
*  **Corporate Headquarters**: A centralized control point that overlooks and manages the functioning of all branches.  It includes a dedicated server room to securely store data for all branches.
* **Routing Implementation**:
    *  **EIGRP**: Enhanced Interior Gateway Routing Protocol is implemented to manage connectivity between the branches and corporate headquarters.  This provides fast convergence, redundancy, and efficient path selection using bandwidth and delay metrics.
    *  **Static/Dynamic Routing**: Utilized alongside default gateways to manage internal routing tables and optimize localized flow.
*  **IP Addressing & Subnetting**: A comprehensive static IP addressing scheme and subnetting strategy is applied to optimize the network across all computers, printers, and peripherals.

---

## ⚙️ Network Components

| Component | Function/Description |
| :--- | :--- |
| **Cisco 2811 Routers** |  Handles inter-branch and HQ data flow, configured with EIGRP. |
| **Switches** |  Facilitates localized branch connections. |
| **End Devices** |  PCs, Laptops, and Printers assigned static IPs. |
| **Central/Local Servers** |  HQ servers handle global data; local servers handle branch data. |

---

## 🛠️ Tech Stack & Methodologies

*  **Software**: Cisco Packet Tracer 
*  **Routing Protocols**: EIGRP, Static Routing, RIP
* **Validation**:
    *  **PDU Tracking**: Tracing Protocol Data Unit headers and payloads across the network.
    *  **ICMP Testing**: Documented testing and troubleshooting using ping commands to ensure connectivity.

---

## 🚀 Installation & Simulation

**Prerequisites**
You will need [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer) installed on your system.

**Steps to Run**
1. Clone the repository via terminal or Git Bash:
```bash
git clone [https://github.com/Arslan-SoftwareEngineer/Banking-Network-Simulation.git](https://github.com/Arslan-SoftwareEngineer/Banking-Network-Simulation.git)
cd Banking-Network-Simulation
```
2. Open Cisco Packet Tracer.
3. Navigate to `File > Open` and select the `Banking_Network.pkt` file.
4. Access the CLI of any router (e.g., `Router3` or `Router0`) to view the EIGRP configurations.
5. Open the `Command Prompt` on any end device (e.g., `PC0` or `PC5`) and use the `ping` command (e.g., `ping 192.168.16.5`) to verify end-to-end connectivity.
6. Use the Simulation tab to view PDU sending events in real-time.
