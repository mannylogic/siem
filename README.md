# 🌍 Global Threat Detection with Azure Sentinel

## 📌 Project Overview

This project demonstrates how to set up a **threat detection and visualization system** using Microsoft Azure. A virtual machine was intentionally exposed to the internet, simulating a realistic attack surface. All security logs were collected, centralized, and analyzed using **Azure Log Analytics** and **Microsoft Sentinel**.

Using a custom **geolocation watchlist**, we enriched the data from failed login attempts and visualized the geographic origin of suspicious IP addresses.



## 🛠️ Tech Stack

- **Microsoft Azure**
  - Azure Virtual Machine (Windows)
  - Azure Network Security Group (NSG)
  - Log Analytics Workspace
  - Azure Monitor Agent
  - Microsoft Sentinel
- **KQL (Kusto Query Language)**
- **Watchlist (CSV Upload)**
- **Geolocation/IP Intelligence**


## 🧠 What Was Implemented

1. **Azure Infrastructure Setup**  
   - Tenant, Subscription, Resource Group  
   - Virtual Network & Subnet  
   - Virtual Machine exposed to the internet via NSG rules  

2. **Logging & Monitoring**  
   - Deployed **Azure Monitor Agent** to the VM  
   - Forwarded logs to **Log Analytics Workspace**  

3. **Threat Detection with Sentinel**  
   - Connected Sentinel to Log Analytics  
   - Uploaded a **geolocation watchlist** of IP blocks by region  
   - Wrote KQL queries to detect and filter **failed logons** from the logs  

4. **Visualization**  
   - Used IP correlation to map attack origin across countries  
   - Created dashboards showing **top attacker locations**

