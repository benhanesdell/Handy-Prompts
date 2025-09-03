Here's how to **install and configure the PPE Detection Module** from EpicIO in your **isolated hospital innovation lab environment** using the Dell XR8000:

---

## 🧰 PPE Detection Module: Installation & Setup Guide

### 🔍 Overview
EpicIO’s **DeepInsights™ AI platform** includes a PPE Detection Module that can identify whether individuals are wearing required protective gear (e.g., masks, gloves, gowns, face shields). This module is part of the **DeepVision** video analytics suite and is compatible with edge deployments like the Dell XR8000[1](https://www.epicio.com/video/).

---

### 📦 Where to Get It

- **Download Location**:  
  EpicIO provides software packages for Dell environments via their asset portal. For Dell XR8000, use:  
  `https://assets.epicio.com/dell/epic_stack_v2.2.tar.gz`  
  This archive includes DeepVision, DeepInsights™, and relevant modules[2](https://infohub.delltechnologies.com/en-us/l/dell-nativeedge-for-retail-quick-start-guide-with-epic-io/day-0-planning-and-prerequisite-preparation/5/).

- **Support Page**:  
  Visit the [EpicIO Installation Guide](https://www.epicio.com/installation-guide/) for hardware-specific instructions and contact support at `support@epicio.com` for module access[3](https://www.epicio.com/installation-guide/).

---

### ⚙️ Dependencies & System Requirements

| Component | Requirement |
|----------|-------------|
| **Server** | Dell XR8000 with GPU (NVIDIA L4 or A2 recommended) |
| **OS** | Ubuntu 20.04 LTS or Windows Server 2019 |
| **Cameras** | IP cameras (ONVIF-compliant preferred) |
| **Network** | Isolated VLAN with static IPs |
| **Software** | Docker, NVIDIA drivers, EpicIO DeepVision stack |

---

### 🛠️ Installation Steps

#### 1. **Prepare the Environment**
- Ensure Dell XR8000 is powered and connected to isolated network.
- Assign static IPs to cameras and server.
- Install Docker and NVIDIA GPU drivers.

#### 2. **Download and Extract Software**
```bash
wget https://assets.epicio.com/dell/epic_stack_v2.2.tar.gz
tar -xzvf epic_stack_v2.2.tar.gz
cd epic_stack_v2.2
```

#### 3. **Deploy DeepVision Stack**
```bash
docker-compose up -d
```
- This launches DeepVision, DeepInsights™, and the PPE Detection Module.

#### 4. **Configure Cameras**
- Access DeepVision dashboard via browser (`http://<XR8000-IP>:8080`)
- Add cameras using ONVIF or RTSP streams.
- Define detection zones (e.g., entryways, PPE-required areas).

#### 5. **Enable PPE Detection**
- In the DeepInsights™ dashboard, activate the **PPE Detection Module**.
- Select PPE types to monitor (mask, gloves, gown, face shield).
- Set alert thresholds and notification preferences.

---

### 🧪 Validation & Testing

1. Simulate entry with full PPE.
2. Simulate entry missing one item (e.g., no mask).
3. Observe dashboard alerts and logs.
4. Adjust detection sensitivity if needed.

---

### 🧯 Troubleshooting Tips

| Issue | Fix |
|------|-----|
| No camera feed | Check RTSP/ONVIF stream and firewall rules |
| PPE not detected | Recalibrate detection zones and lighting |
| Module not loading | Verify Docker containers and GPU availability |

---

Would you like a **camera placement diagram** or a **Docker config template** for this setup?
