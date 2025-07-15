## 🌐 Part 6: **Azure Networking Services**

Azure Networking provides secure, scalable, and high-performance infrastructure for connecting and managing your resources in the cloud. Understanding Azure networking is crucial for setting up communication between virtual machines, services, and the internet.

---

### 🔹 **1. Virtual Networks (VNet)**

- A **Virtual Network** is a logically isolated network in Azure.
- Similar to on-premises networks but hosted in the cloud.
- Supports subnets, custom IP address ranges, DNS, route tables, etc.

> 🔧 VNets allow **communication between Azure resources**, **on-premises**, and **the internet**.

---

### 🔹 **2. Subnets, NSGs, ASGs**

#### **Subnets**
- Divide a VNet into **smaller segments**
- Help isolate resources by workload or security level

#### **NSGs (Network Security Groups)**
- Act as **firewalls** at the subnet or NIC level
- Allow or deny **inbound/outbound traffic**
- Control access using **rules** based on IP, port, protocol

#### **ASGs (Application Security Groups)**
- Group VMs with similar functions
- Simplify NSG rule management by targeting **groups instead of individual IPs**

---

### 🔹 **3. Load Balancers & Application Gateway**

#### **Azure Load Balancer**
- Distributes traffic across **VMs** in a load-balanced set
- Supports **TCP/UDP** traffic at **Layer 4**
- Available in **Basic** and **Standard** SKUs

#### **Azure Application Gateway**
- Works at **Layer 7** (HTTP/HTTPS)
- Includes features like **URL-based routing**, **SSL termination**, and **Web Application Firewall (WAF)**

> 🌐 Use Load Balancer for network-level traffic; use App Gateway for web apps and advanced routing.

---

### 🔹 **4. VPN Gateway & VNet Peering**

#### **VPN Gateway**
- Connects **on-premises networks** to Azure over **IPSec/IKE VPN tunnels**
- Supports **site-to-site**, **point-to-site**, and **VNet-to-VNet** connections

#### **VNet Peering**
- Connects two VNets for **private traffic routing**
- Works **within** or **across** regions
- Low-latency, high-throughput communication

> 🔒 Peered VNets appear as part of the **same network** for traffic routing.

---

### 📌 Best Practices

- Use **NSGs** to control access at both subnet and NIC levels
- Use **Bastion** for secure VM access without exposing public IPs
- Design for **HA** using Availability Zones and Load Balancers
- Monitor with **Network Watcher** and **Azure Monitor**
- Avoid overlapping IP ranges for VNet peering

---

> ✅ Azure Networking is the foundation for secure and scalable architectures. Mastering it helps ensure your infrastructure is both robust and protected.
