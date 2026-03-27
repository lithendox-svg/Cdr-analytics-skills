---
name: llm-api-engine
description: "Build LLM-powered applications and call analytics dashboards with advanced KPI tracking, agent insights, automation, and performance optimization."
license: Complete terms in LICENSE.txt
---

# LLM API Engine + CDR Analytics

A professional skill designed to build scalable AI-powered applications and advanced call analytics dashboards with real-time insights, KPI tracking, and performance optimization.

---

## 🚀 Core Capabilities

### 🔹 LLM Application Development
- Build AI-powered applications using APIs and SDKs
- Design workflows, automation, and agent systems
- Enable structured outputs and intelligent processing

### 🔹 Call Analytics & Dashboard System
- Performance KPIs: Total calls, answered rate, missed rate, AHT, occupancy
- Agent Performance Management: Leaderboard and efficiency tracking
- Advanced Visual Analytics: Hourly trends, call distribution, patterns
- Dynamic Filtering: Date, agent, route, status, segment
- Category Intelligence: Segment-level analysis
- Granular Insights: Sub-category performance tracking
- Agent Deep-Dive: Individual behavioral and performance insights
- Real-Time Data Sync: API / automation integration
- Customizable Interface: Multiple themes support

---

## 📊 Business Impact

- Enables data-driven decision making with real-time insights
- Improves agent productivity by identifying gaps
- Enhances operational efficiency through clear analytics
- Supports strategic planning with actionable data
- Identifies high and low-performing segments quickly

---

## ⚙️ Default Behavior

- Provide structured KPI summaries
- Highlight key insights and anomalies
- Suggest actionable improvements
- Use efficient and scalable solutions
- Keep responses clear and professional
- Prefer production-ready code

---

## 🧠 When to Use This Skill

Trigger when:
- Working with AI APIs or SDKs
- Building dashboards or analytics tools
- Analyzing call center / CDR data
- Creating automation workflows or agents
- Designing KPI tracking systems

Do NOT trigger when:
- General coding without AI or analytics
- Basic frontend/UI-only tasks
- Non-data-related queries

---

## 🧩 Architecture Guidance

### 1. LLM Layer
- Handle API communication
- Process prompts and responses
- Generate insights and summaries

### 2. KPI & Dashboard Layer
- Aggregate call data into metrics
- Visualize hourly, daily, and segment-wise trends
- Highlight today's performance

### 3. Filtering & Drilldown Layer
- Multi-level filters (date, agent, route, status, segment)
- One-click status filtering
- Agent-level drilldown with detailed insights

### 4. Agent Intelligence Layer
- Rank agents based on performance
- Calculate answered, missed, AHT
- Identify strengths and improvement areas

### 5. Workflow / Agent Layer
- Multi-step processing systems
- Automation pipelines
- Tool-based or agent-based execution

---

## 🔧 Development Strategy

- Start simple, then scale complexity
- Use modular and reusable components
- Avoid duplicating logic
- Keep code clean and maintainable
- Separate data, logic, and UI layers

---

## 📈 Optimization Tips

- Use streaming for large responses
- Set proper token limits
- Minimize redundant calculations
- Cache stable prompts/data
- Optimize chart rendering and filtering

---

## ⚠️ Common Pitfalls

- Overengineering simple use cases
- Using agents unnecessarily
- Poor data validation
- Incorrect filter logic
- Excessive API usage causing latency

---

## 🧪 Best Practices

- Validate all inputs and outputs
- Structure responses clearly (KPI → Insight → Action)
- Maintain consistent naming conventions
- Log important operations
- Design for scalability

---

## 💻 Code Examples

### 🔹 JavaScript (Dashboard KPI Calculation)
```javascript
const total = data.length;
const answered = data.filter(d => d.status === 'ANSWERED').length;
const missed = total - answered;
const rate = total ? (answered / total * 100).toFixed(1) + '%' : '0%';

console.log({ total, answered, missed, rate });
