# 🔍 Automated SEO Keyword Rank Tracker via Bright Data MCP & GPT-5.2

An advanced, AI-driven **n8n workflow** designed to automate SEO keyword tracking[cite: 2]. By leveraging **Bright Data's Model Context Protocol (MCP)** integration alongside **GPT-5.2**, this pipeline simulates hyper-realistic user searches to bypass CAPTCHAs, scrapes the top 5 Google Search Engine Results Page (SERP) positions, and dynamically updates an analytics tracking dashboard in **Google Sheets**[cite: 2].

---

## 🛠️ How It Works

The workflow operates seamlessly across 3 main architectural zones:

### 1. 🟦 Input & Trigger Configuration
* **🕒 Scheduled Trigger:** Starts automatically on a custom schedule (Daily for volatile tracking or Weekly for long-term trends)[cite: 2].
* **📝 Target Parameter Definition:** Dynamically stores search tracking requirements such as target keywords (e.g., `"best running shoes"`) and domain footprints[cite: 2].

### 2. 🟨 Smart SERP Scraping with AI Agent
* **🤖 SERP Scraper Agent:** A localized AI reasoning agent operating on LangChain frameworks within n8n[cite: 2].
* **🧠 GPT-5.2 AI Brain:** Formulates search contextualization parameters via the OpenAI Chat Model nodes[cite: 2].
* **🌐 Bright Data MCP Client:** Connects natively to real mobile proxy network protocols to anonymously query Google Search, avoiding strict cloud-scraping blocks[cite: 2].
* **🧾 Structured Output Parser:** Utilizes an auto-fixing parser mapping schemas directly into standard data models containing: `rank`, `title`, `url`, and `description`[cite: 2].

### 3. 🟩 Rank Logging & Reporting
* **🧠 Format SERP Results:** A JavaScript code engine that converts the bulk array into decoupled unique stream instances[cite: 2].
* **📊 Log to Google Sheets:** Commits streaming parameters to individual spreadsheet columns for immediate graphing and monitoring[cite: 2].

---

## 📸 Workflow Architecture

<img width="440" height="367" alt="image" src="https://github.com/user-attachments/assets/c3955f07-ed38-476b-9ed2-8e90f5c719e9" />


---

## 🎯 Key Extracted Metadata

The following properties are securely parsed and structuralized per execution:
* 🔟 **Rank:** Exact search performance positioning ($1\rightarrow5$)[cite: 2].
* 🔗 **URL:** Clean destination canonical landing page links[cite: 2].
* ✍️ **Title:** Page index headers captured from SERP viewports[cite: 2].
* 📄 **Description:** Meta snippets serving contextual content representations[cite: 2].

---

## 🚀 Getting Started

### Prerequisites
* A running **n8n** instance with LangChain node options available[cite: 2].
* An **OpenAI API Key** with access authorization for advanced GPT models[cite: 2].
* An active **Bright Data MCP** environment profile connection[cite: 2].
* Authenticated access to a target **Google Sheets** instance[cite: 2].

### Installation Steps
1. **Download the Blueprint:** Grab the `Generate Leads with Google Maps - AlexK1919.json` file from this repository.
2. **Import to Canvas:** Go to your n8n dashboard, select the options dropdown menu in the upper right workspace sector, and import the blueprint file[cite: 2].
3. **Establish Credentials:** 
   * Connect your OpenAI account API keys inside the `OpenAI Chat Model` nodes[cite: 2].
   * Set up connection endpoints on the `MCP Client` instance[cite: 2].
   * Connect your Google OAuth workspace properties to the final reporting spreadsheet[cite: 2].
4. **Deploy & Track:** Flip the active trigger state toggle to automate your competitive search rank reports[cite: 2]!
