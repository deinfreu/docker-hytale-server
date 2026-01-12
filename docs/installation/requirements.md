---
layout: default
title: "Requirements"
parent: "📥 Installation"
nav_order: 1
---

## 📋 Requirements & Licensing

Before deploying the container, ensure your environment meets the following hardware and licensing requirements.

### 🔑 Hytale License
Because Hytale requires a valid license to access server binaries, this container does not come pre-packaged with the game files.
* **Authentication:** You must provide your Hytale license credentials to the container via environment variables.
* **Update Notifications:** Every night at **00:00 (Midnight)**, the tool performs an automated check. If a new version is found, it will **alert you in the logs** so you can decide when to manually trigger the update process.