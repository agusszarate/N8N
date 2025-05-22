# 🧠 n8n Personal - Expense Tracking via WhatsApp

This repository contains a minimal setup to deploy an [n8n](https://n8n.io/) instance on the cloud (e.g., Render) with workflows such as personal expense tracking via WhatsApp and Google Sheets integration.

## 🚀 Quick Deployment on Render

1. Create a new service at [Render](https://render.com):
   - Choose **Web Service**
   - Select this repository from your GitHub account
   - Configure as follows:
     - **Environment**: Docker
     - **Start Command**: `n8n`
     - **Port**: `5678`
2. Wait for the service to build and access your n8n instance at the public URL provided by Render.

## 🧰 Contents

- `Dockerfile`: Minimal n8n image ready to run.
- `workflows/`: Folder to store backups or versions of your exported workflows (`.json`).
  - Example: `expense-tracker.json`

## 🧠 What is n8n?

n8n is a workflow automation tool with low-code/no-code capabilities. You can connect services like WhatsApp, Google Sheets, Telegram, APIs, and more.

## 📂 How to Export Your Workflows

1. In n8n, click on the three dots at the top right.
2. Select **Export**.
3. Save the `.json` file into the `workflows/` folder of this repo.

## ⚠️ Security

Do **NOT** commit sensitive credentials (tokens, client secrets, passwords) to the repository. Use n8n's credential management system instead.

---

## ✨ License

MIT License. Made with ❤️ by you for personal use.
