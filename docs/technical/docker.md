---
layout: default
title: "Docker"
parent: "⚙️ Technical Info"
nav_order: 1
---

# 🐳 Docker Configuration Reference

The Hytale server container is highly configurable through environment variables. These allow you to tune performance, security, and automation without modifying the internal container files.

## 🔑 Required Variables

| Variable | Description | Default |
| :--- | :--- | :--- |
| `EULA` | Must be set to `TRUE` to indicate agreement with the Hytale EULA. | `FALSE` |

---

## ⚙️ Core Server Settings

| Variable | Description | Default |
| :--- | :--- | :--- |
| `JAVA_FLAG` | Enter the java startup flags here | `-` |
| `TZ` | The [Timezone identifier](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones) for server logs. | `UTC` |
| `DEBUG` | Set to `TRUE` to enable diagnostic scripts and verbose logging. | `FALSE` |
| `SERVER_PORT` | The primary UDP port for game traffic. | `5520` |
| `QUERY_PORT` | Port used for server list queries and heartbeats. | `25565` |
| `JAVA_OPTS` | Additional flags for the JVM (Expert use only). | `(Empty)` |

---

## ⚙️ Hytale Settings

| Variable | Description | Default |
| :--- | :--- | :--- |
| `HYTALE` | - | - |

---

## 📂 Volume Mapping (Persistence)

To ensure your world, player data, and configurations are saved when the container restarts, you **must** map a volume to the internal working directory.

| Container Path | Purpose |
| :--- | :--- |
| `/home/container` | Main directory containing world files, logs, and configs. |