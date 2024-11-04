# Getting Started with SIEM Tools: Splunk & Microsoft Sentinel

## Introduction

This guide introduces two popular Security Information and Event Management (SIEM) tools: **Splunk** and **Microsoft Sentinel**. SIEM tools are essential for monitoring and analyzing security data across various sources, providing real-time alerts, and helping organizations respond to potential threats.

### Contents
- [What is SIEM?](#what-is-siem)
- [Setting Up Splunk](#setting-up-splunk)
  - [Installation](#installation)
  - [Basic Configuration](#basic-configuration)
- [Setting Up Microsoft Sentinel](#setting-up-microsoft-sentinel)
  - [Installation](#installation)
  - [Basic Configuration](#basic-configuration)
- [Basic Operations](#basic-operations)
  - [Adding Data Sources](#adding-data-sources)
  - [Creating Alerts](#creating-alerts)
  - [Dashboards and Reporting](#dashboards-and-reporting)
- [Further Learning](#further-learning)

---

## What is SIEM?

**SIEM** stands for **Security Information and Event Management**. It's a security tool that collects and analyzes activity from various sources across an organization’s IT infrastructure. SIEM tools enable real-time monitoring, event correlation, and incident detection, providing insights into potential threats and security incidents.

## Setting Up Splunk

Splunk is a powerful platform for collecting, analyzing, and visualizing data from various sources.

### Installation

1. **Download Splunk**:
   - Visit the [official Splunk download page](https://www.splunk.com/en_us/download/splunk-enterprise.html).
   - Choose the appropriate installer for your operating system (Windows, macOS, or Linux).

2. **Install Splunk**:
   - **Windows**: Run the `.msi` installer and follow the prompts.
   - **macOS**: Run the `.dmg` file and follow the instructions.
   - **Linux**:
     ```bash
     sudo dpkg -i splunk-package-name.deb  # Debian/Ubuntu
     sudo rpm -ivh splunk-package-name.rpm  # Red Hat/CentOS
     ```

3. **Start Splunk**:
   - Run the command:
     ```bash
     ./splunk start
     ```
   - Open a browser and go to `http://localhost:8000` to access the Splunk dashboard.

4. **Set Up Admin Account**:
   - Follow the setup wizard to create your admin credentials.

### Basic Configuration

- **Add Data Sources**:
  - Navigate to **Settings > Add Data**.
  - Follow the wizard to connect log files, directories, network data, or cloud data.
- **Define Indexes**:
  - Set up indexes in **Settings > Indexes** to organize data types (e.g., `web_logs`, `system_logs`).

## Setting Up Microsoft Sentinel

Microsoft Sentinel is a scalable, cloud-native SIEM and SOAR (Security Orchestration Automated Response) solution for intelligent security analytics.

### Installation

1. **Prerequisites**:
   - Ensure you have an **Azure Subscription**. Set up a free account [here](https://azure.microsoft.com/free/).

2. **Set Up Sentinel**:
   - Open the Azure Portal.
   - In **Azure Sentinel**, create a Sentinel instance by selecting your workspace and region.

### Basic Configuration

- **Connect Data Sources**:
  - In the Azure Sentinel dashboard, go to **Data connectors**.
  - Choose from connectors like Azure Active Directory, Office 365, Firewalls, or custom logs, and follow the setup steps.

## Basic Operations

### Adding Data Sources

- **Splunk**: Use the **Add Data** wizard to connect data sources such as directories, cloud services, or databases.
- **Sentinel**: Use **Data connectors** to add Azure-native data, custom logs, or external sources.

### Creating Alerts

- **Splunk**:
  - Go to **Search & Reporting**, create a query for your target events, save the search, and enable alerts for specific conditions.

- **Microsoft Sentinel**:
  - Navigate to **Analytics**, use rule templates, or create custom rules to set alerts for conditions like login failures or suspicious IP activity.

### Dashboards and Reporting

- **Splunk**:
  - Use **Dashboards** to create custom visualizations based on your data.
  - Add charts, tables, and other visualizations for data insights.

- **Sentinel**:
  - In **Workbooks**, select from pre-built templates or create custom workbooks for visualizing alerts, incident trends, and other metrics.

## Further Learning

- **Splunk**:
  - [Splunk Docs](https://docs.splunk.com/Documentation/Splunk)
  - [Splunk Community](https://community.splunk.com/)

- **Microsoft Sentinel**:
  - [Microsoft Sentinel Documentation](https://docs.microsoft.com/azure/sentinel/)
  - [Microsoft Learn](https://learn.microsoft.com/azure/sentinel/)

---

This guide covers the essentials for getting started with Splunk and Microsoft Sentinel. As you progress, explore more advanced features in each tool to expand your skills in security monitoring and incident response.

