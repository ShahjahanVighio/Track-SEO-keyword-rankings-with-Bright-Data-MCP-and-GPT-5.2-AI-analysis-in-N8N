# 🔍 Automated SEO Keyword Rank Tracker via Bright Data MCP & GPT-5.2

An advanced, AI-driven **n8n workflow** designed to automate SEO keyword tracking. By leveraging **Bright Data's Model Context Protocol (MCP)** integration alongside **GPT-5.2**, this pipeline simulates hyper-realistic user searches to bypass CAPTCHAs, scrapes the top 5 Google Search Engine Results Page (SERP) positions, and dynamically updates an analytics tracking dashboard in **Google Sheets**.

---

## 🛠️ How It Works

The workflow operates seamlessly across 3 main architectural zones:

### 1. 🟦 Input & Trigger Configuration
* **🕒 Scheduled Trigger:** Starts automatically on a custom schedule (Daily for volatile tracking or Weekly for long-term trends).
* **📝 Target Parameter Definition:** Dynamically stores search tracking requirements such as target keywords (e.g., `"best running shoes"`) and domain footprints.

### 2. 🟨 Smart SERP Scraping with AI Agent
* **🤖 SERP Scraper Agent:** A localized AI reasoning agent operating on LangChain frameworks within n8n.
* **🧠 GPT-5.2 AI Brain:** Formulates search contextualization parameters via the OpenAI Chat Model nodes.
* **🌐 Bright Data MCP Client:** Connects natively to real mobile proxy network protocols to anonymously query Google Search, avoiding strict cloud-scraping blocks.
* **🧾 Structured Output Parser:** Utilizes an auto-fixing parser mapping schemas directly into standard data models containing: `rank`, `title`, `url`, and `description`.

### 3. 🟩 Rank Logging & Reporting
* **🧠 Format SERP Results:** A JavaScript code engine that converts the bulk array into decoupled unique stream instances.
* **📊 Log to Google Sheets:** Commits streaming parameters to individual spreadsheet columns for immediate graphing and monitoring.

---

## 📸 Workflow Architecture

<img width="440" height="367" alt="image" src="https://github.com/user-attachments/assets/c3955f07-ed38-476b-9ed2-8e90f5c719e9" />


---

## 🎯 Key Extracted Metadata

The following properties are securely parsed and structuralized per execution:
* 🔟 **Rank:** Exact search performance positioning ($1\rightarrow5$).
* 🔗 **URL:** Clean destination canonical landing page links.
* ✍️ **Title:** Page index headers captured from SERP viewports.
* 📄 **Description:** Meta snippets serving contextual content representations.

---

## 🚀 Getting Started

### Prerequisites
* A running **n8n** instance with LangChain node options available.
* An **OpenAI API Key** with access authorization for advanced GPT models.
* An active **Bright Data MCP** environment profile connection.
* Authenticated access to a target **Google Sheets** instance.

### Installation Steps
1. **Download the Blueprint:** Grab the `Generate Leads with Google Maps - AlexK1919.json` file from this repository.
2. **Import to Canvas:** Go to your n8n dashboard, select the options dropdown menu in the upper right workspace sector, and import the blueprint file.
3. **Establish Credentials:** 
   * Connect your OpenAI account API keys inside the `OpenAI Chat Model` nodes.
   * Set up connection endpoints on the `MCP Client` instance.
   * Connect your Google OAuth workspace properties to the final reporting spreadsheet.
4. **Deploy & Track:** Flip the active trigger state toggle to automate your competitive search rank reports[cite: 2]!
