# ☁️ Weather Forecast Cloud Flow — Power Automate + Copilot

> **A cloud flow built with Microsoft Copilot in Power Automate that fetches real-time weather forecasts for agent-driven customer interactions.**

---

## 📌 Project Overview

This project demonstrates how to use **Microsoft Copilot in Power Automate** to design and automate a cloud flow using natural language prompts. The flow enables an AI agent to fetch today's weather forecast for any city and ZIP code dynamically, and return structured data back to the calling agent.

The workflow was built as part of a hands-on learning exercise focused on:
- AI-assisted flow creation using Copilot
- Agent-callable trigger configuration
- Dynamic data input/output with the MSN Weather connector

---

## 🎯 Learning Objectives

- Use **natural language prompts** to design workflows in Power Automate
- Configure **triggers** (agent-callable) and **actions** (weather fetch, response)
- Test and validate the automation end-to-end

---

## 🧩 Flow Architecture

```
[When an agent calls the flow]
        ↓
[Get forecast for today]   ← MSN Weather Connector
        ↓
[Respond to the agent]     ← Returns structured weather output
```

---

## ⚙️ Input Parameters

| Parameter | Type   | Description                  |
|-----------|--------|------------------------------|
| `City`    | Text   | Name of the target city      |
| `ZIP code`| Text   | ZIP code of the target city  |

---

## 📤 Output Parameters

| Parameter        | Type   | Description                          |
|------------------|--------|--------------------------------------|
| `day_summary`    | Text   | Summary of the day's weather          |
| `location`       | Text   | Resolved location name                |
| `chance_of_rain` | Number | Probability of rain (as a percentage) |

---

## 🛠️ Technologies Used

| Tool / Service             | Purpose                              |
|----------------------------|--------------------------------------|
| Microsoft Power Automate   | Cloud flow hosting and orchestration |
| Microsoft Copilot (PA)     | AI-assisted flow generation          |
| MSN Weather Connector      | Real-time weather data source        |
| Power Platform Agent       | Flow caller via agent trigger        |

---

## 🚀 How to Use

1. **Import or recreate** the flow in your Power Automate environment
2. Ensure the **MSN Weather connector** is authorized
3. Connect an **AI agent** (e.g., Copilot Studio agent) to call this flow
4. Pass `City` and `ZIP code` as input parameters
5. Receive `day_summary`, `location`, and `chance_of_rain` as outputs

---

## 🧪 Testing

The flow was manually tested using the **Test** feature in Power Automate:

- **Input:** City name + ZIP code provided manually
- **Result:** Flow ran successfully ✅
- **Output verified:** Weather details returned via the `Respond to the agent` action

> See screenshot: flow diagram showing all 3 steps completing with green checkmarks.

---

## ✅ Status

| Task                              | Status      |
|-----------------------------------|-------------|
| Flow created via Copilot          | ✅ Complete |
| Agent trigger configured          | ✅ Complete |
| Input parameters defined          | ✅ Complete |
| MSN Weather action configured     | ✅ Complete |
| Respond to agent action added     | ✅ Complete |
| Flow tested and validated         | ✅ Complete |
| Flow saved and published          | ✅ Complete |

---

## 👤 Author

**Rofiah Kehinde**  
Power Platform learner | Cloud Flow automation exercise

---

## 📄 License

This project was created for educational purposes as part of a Microsoft Power Platform learning module.
