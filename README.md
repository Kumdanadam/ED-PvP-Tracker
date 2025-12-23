# 🚀 Elite Dangerous PvP Tracker

**ED PvP Tracker** is a powerful, lightweight, Python-based tool designed for Elite Dangerous PvP pilots. It automatically scans your game journal logs to track player kills, generates detailed HTML reports, and posts stylish combat summaries to your Discord server via Webhooks.

> **Created by Cmdr Yu-gen**

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![Elite Dangerous](https://img.shields.io/badge/Game-Elite%20Dangerous-orange?style=for-the-badge)
![Discord](https://img.shields.io/badge/Integration-Discord%20Webhook-5865F2?style=for-the-badge)

## ✨ Key Features

* **📊 Comprehensive Tracking:** Scans your logs to find every PvP kill you've ever made.
* **🤖 Discord Integration:**
    * **All Time / Daily Reports:** Posts detailed kill lists with total kill counts (in **bold**).
    * **Last Kill Alert:** A special, high-visibility "Target Destroyed" card for instant flexing.
    * **Smart Formatting:** Handles long kill lists automatically without breaking Discord's character limits.
* **📑 HTML Reports:** Generates sorting-friendly HTML tables saved directly to your Desktop. Columns include:
    * Date & Time
    * Pilot Name (with Inara Link)
    * Combat Rank
    * **Ship Type** (e.g., FDL, Cutter)
    * Squadron (with Inara Link)
    * Powerplay Allegiance
* **⚡ Powerplay Awareness:** Automatically detects the victim's Power (e.g., *Arissa Lavigny-Duval*, *Yuri Grom*) and applies color-coded accents to Web reports and Discord embeds.
* **🛡️ Dynamic Filtering (Friendly Fire):**
    * Exclude specific Squadrons (e.g., your own wingmates) from reports.
    * Easy-to-use input box in the GUI (e.g., `XXXX, XXXX`).
* **🎨 Modern Dark UI:** A sleek, user-friendly interface built with Tkinter.
* **📂 Smart Path Finding:** Automatically detects your Desktop path, even if it's synced with OneDrive.

## 🛠️ Installation & Usage

### Option 1: Running the Executable (.exe)
If you have the compiled `.exe` file:
1.  Download `ED_PvP_Tracker.zip`.
2.  Extract `ED_PvP_Tracker.exe`.
3.  Double-click to run (No installation required).
4.  Enter your settings (see below) and start tracking.

When you open the application, you will see a configuration panel:

1.  **Webhook URL:** Paste your Discord Webhook URL here. (See *How to get a Webhook* below).
2.  **Avatar URL (Optional):** Link to an image you want to appear as the "Author" icon in Discord messages.
3.  **Excluded Squadrons:** Enter the tags of squadrons you want to ignore (e.g., friendly fire).
    * *Format:* Separate with commas (e.g., `XXXX, XXXX`).
    * *Note:* Not case sensitive.

*Configuration is automatically saved to `pvp_tracker_config.json` in your user folder.*

## 🎮 How to Get a Discord Webhook

1.  Open **Discord** and go to the server where you want the reports.
2.  Go to **Server Settings** > **Integrations** > **Webhooks**.
3.  Click **New Webhook**.
4.  Name it (e.g., "Kill Tracker") and choose the channel.
5.  Click **Copy Webhook URL**.
6.  Paste this URL into the application.
