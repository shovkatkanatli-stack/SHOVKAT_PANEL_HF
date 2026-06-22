---
title: Luffy Panel
emoji: 🏴‍☠️
colorFrom: yellow
colorTo: gray
sdk: docker
pinned: false
license: mit
app_port: 7860
---

# 🏴‍☠️ Luffy Panel — Hugging Face Edition

VLESS Proxy Gateway Management Panel — now running on Hugging Face Spaces.

## Features

- 🌐 **VLESS Tunnel** — WebSocket-based VLESS proxy gateway
- 📊 **Live Dashboard** — Real-time traffic stats, connections, CPU/RAM
- 🔗 **Link Management** — Create/edit/delete VLESS configs with quotas & expiry
- 📱 **Subscription** — Generate VLESS subscription links for clients
- 🛡️ **Auth System** — Password-protected admin panel
- 🌍 **Custom Addresses** — Add custom IPs for multi-server configs
- 🎨 **Dual Theme** — Dark/Light mode with English & Persian (فارسی)

## Environment Variables

| Variable | Default | Description |
|---|---|---|
| `ADMIN_PASSWORD` | `admin` | Panel login password |
| `SECRET_KEY` | auto-generated | Session encryption key |

Set these in your Space Settings → Repository secrets.

## Usage

1. Deploy to Hugging Face Spaces as a Docker Space
2. Open your Space URL
3. Login with `admin` / your custom password
4. Create links and share VLESS configs

> ⚠️ **Note:** Hugging Face Spaces sleep after 48h of inactivity (free tier). The panel includes a keep-alive mechanism.

## Deploy on Hugging Face

1. Go to [huggingface.co/new-space](https://huggingface.co/new-space)
2. Choose **Docker** as the Space SDK
3. Upload these files or connect your GitHub repo
4. Set `ADMIN_PASSWORD` secret (optional)
5. Your panel will be live at `https://{username}-luffy-panel.hf.space`

## Credits

Originally built for Render/Railway. Adapted for Hugging Face Spaces by استاد ترید.
