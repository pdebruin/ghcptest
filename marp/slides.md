---
marp: true
theme: student-hub
paginate: true
---

# Welcome to ghcptest

A GitHub Copilot Testing Repository

---

# What is Marp?

**Marp** (Markdown Presentation Ecosystem) is a tool to create beautiful slide decks using Markdown.

## Key Features

- 📝 Write presentations in Markdown
- 🎨 Multiple themes available
- 🚀 Export to HTML, PDF, and PowerPoint
- 🔧 Highly customizable

---

# How to Create an Azure AI Foundry Instance 1/2

Azure AI Foundry (formerly Azure AI Studio) provides a unified experience for building AI solutions.

## Steps using Azure CLI 

1. **Install the Azure CLI extension**
   ```bash
   az extension add --name ml
   ```

2. **Create a resource group** (if needed)
   ```bash
   az group create --name <resource-group-name> --location <location>
   ```

---

# How to Create an Azure AI Foundry Instance 2/2

## Steps using Azure CLI

3. **Create an Azure AI Foundry hub**
   ```bash
   az ml workspace create --kind hub \
     --resource-group <resource-group-name> \
     --name <hub-name>
   ```

4. **Create a project within the hub**
   ```bash
   az ml workspace create --kind project \
     --resource-group <resource-group-name> \
     --name <project-name> \
     --hub-id <hub-resource-id>
   ```

**Source:** [Microsoft Learn - Azure AI Foundry Documentation](https://learn.microsoft.com/azure/ai-foundry/)

---

# Thank you

http://aka.ms/pieter
