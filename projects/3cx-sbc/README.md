# ☎️ 3CX Cloud PBX and SBC Deployment

This mini-project documents the deployment of a 3CX Cloud PBX system with a self-hosted SBC (Session Border Controller) VM and Grandstream HT802 ATA devices connecting analogue phones.

---

## 🛠 Components

- **3CX Cloud PBX** (self-hosted or free-tier cloud instance)
- **SBC VM** (Debian 11, deployed via Proxmox VM)
- **Grandstream HT802 ATA** (Analogue phone adapters)
- **Home Assistant** (Optional integration for phone-based automation)

---

## 🌐 Architecture

```mermaid
flowchart TD
  Phones(Analog Phones) --> ATA(HT802 ATA)
  ATA --> SBC(SBC VM)
  SBC --> 3CX[3CX Cloud PBX]
  HomeAssistant(Home Assistant) -->|Webhooks/SIP| ATA
