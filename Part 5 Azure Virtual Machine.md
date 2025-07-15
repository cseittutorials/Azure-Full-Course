## 💻 Part 5: **Azure Virtual Machines (VMs)**

**Azure Virtual Machines (VMs)** allow you to run **Windows or Linux-based workloads** in a scalable and flexible environment. VMs are one of the core services in Azure used for hosting applications, testing environments, and migrating on-premises workloads to the cloud.

---

### 🔹 **1. What is an Azure Virtual Machine?**

An **Azure VM** is a **virtualized compute resource** similar to a physical server that runs in Azure's data centers. You can configure:
- The OS (Windows/Linux)
- VM size (CPU, memory)
- Attached disks
- Network interfaces

> ☁️ Azure VMs are part of the **Infrastructure as a Service (IaaS)** model.

---

### 🔹 **2. Creating and Configuring VMs**

You can create VMs via:
- **Azure Portal** (GUI)
- **Azure CLI**
- **Azure PowerShell**
- **ARM Templates or Bicep**

Basic configuration steps:
1. Choose **image** (e.g., Ubuntu, Windows Server)
2. Select **VM size** (e.g., B1s, D2s v3)
3. Configure **authentication** (SSH key or password)
4. Assign **networking** (Virtual Network, Subnet, Public IP)
5. Add **disks** (OS disk + optional data disks)
6. Review and **create**

---

### 🔹 **3. Connecting to VMs**

- **Linux VMs**: Use **SSH** from terminal or Git Bash  
  ```bash
  ssh azureuser@<public-ip>
