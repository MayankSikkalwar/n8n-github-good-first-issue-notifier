# 🚀 Good First Issue Notifier

An automated workflow built with **[n8n.io](https://n8n.io/)** that monitors GitHub repositories for beginner-friendly issues and sends **real-time notifications** to a Telegram channel.

---

## 🎯 Problem Solved  
For developers looking to start contributing to open source, finding the right **“good first issue”** can be difficult.  
Manually checking dozens of repositories is **time-consuming** and inefficient.  

This project automates the discovery process and provides a **streamlined, real-time feed** of contribution opportunities.

---

## 🔧 How It Works  

1. **⏰ Schedule Trigger**  
   A CRON-based trigger runs the workflow at regular intervals (e.g., every hour).  

2. **📂 Fetch Repository Issues**  
   Connects to the **GitHub API** to retrieve all open issues from one or more repositories.  

3. **🔎 Filter for “Good First Issues”**  
   Loops through issues and filters those labeled `good first issue`.  

4. **📝 Format Notification**  
   Extracts key details (Title, Repo Name, URL) and formats them into a clean message.  

5. **📲 Send Telegram Alert**  
   Uses the **Telegram Bot API** to instantly notify subscribers in a Telegram channel.  

---

## 🛠️ Technologies & APIs Used  

- **Core Tool**: [n8n.io](https://n8n.io/)  
- **APIs Integrated**:  
  - GitHub API (fetch issues)  
  - Telegram Bot API (send alerts)  
- **Data Format**: JSON  
- **Core Concepts**: Workflow Automation, API Integration, Webhooks, CRON Scheduling  

---

## ⚙️ Configuration & Setup  

To set up this workflow:  

1. Install or deploy an **n8n instance** (cloud or self-hosted).  
2. Generate a **GitHub Personal Access Token** with `repo` scope.  
3. Create a **Telegram Bot** and obtain:  
   - Bot Token  
   - Channel/Chat ID  
4. Import the workflow JSON file from this repository into your n8n canvas.  
5. Update the GitHub and Telegram credentials with your own tokens.  

---

## 📊 Workflow Visualization  

Here’s a simplified view of the workflow on the n8n canvas:
<img width="1397" height="348" alt="image" src="https://github.com/user-attachments/assets/607e941e-8b59-4dbd-ab0a-33885614bf5c" />


