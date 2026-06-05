---
name: boss-zhipin-greeting
description: Generates highly effective, concise, and data-driven initial greeting messages for HR/recruiters on Boss Zhipin to maximize reply rates.
version: 2.0
---

# Skill: Boss Zhipin High-Response Greeting Generator

## 🎯 Description
A specialized skill for crafting initial outreach messages to HR/recruiters on recruitment platforms like Boss Zhipin. It focuses on bypassing platform noise by using hyper-concise, high-impact, and resume-matched communication.

## ⚡ Trigger Conditions
Activate this skill when the user:
- Asks for help writing or optimizing a greeting/outreach message for HR.
- Provides a job description (JD) and resume to generate a tailored opening.

## 🧠 Core Mindset
**Value-First:** Do not just say "I want a job." Instead, show: **"I have the exact capability to solve your business/technical pain points."**

---

## 📏 The Rules

### Rule 1: Absolute Truthfulness (Zero Extrapolation) ⚖️
Every generated greeting must be 100% traceably true to the user's resume. Any form of inflation or assumption is strictly prohibited.
- **Strict Literal Verification**: Do not mention any company status (e.g., "大厂"), job title/rank (e.g., "专家"), skill, metric, or project role (e.g., "从0到1", "主导") unless the exact word or data is literally written in the resume.
- **No Conceptual Upgrades**: Never round up numbers, upgrade titles, generalize skills, or inflate company scale. If it is not explicitly in `resume.md`, do not write it.

### Rule 2: The "First 8 Characters" Hook (List Preview)
HR scans messages in a list preview. The first 8-10 characters must instantly show matchability with zero fluff.
- **Hook Categories (Choose one)**:
  - *Experience/Title*: `资深前端开发，` / `5年产品经理，` *(For 8+ years, use titles like "资深/专家" instead of exact years to avoid age filtering)*.
  - *Quantifiable Metric*: `主导XX项目，` / `单月业绩销冠，`
  - *Strong Background*: `前大厂技术专家，` / `985硕+大厂算法，`
  - *Core Capability/Pain Point*: `英语可作工作语言，` / `从0到1出海经验，`

### Rule 3: The Three-Line Golden Structure
Every greeting must strictly follow a 3-line format (around 60-80 Chinese characters total):
1. **Line 1 (The Hook):** The hard tag from Rule 2 (visible in preview).
2. **Line 2 (The Proof):** 1-2 concise sentences showing quantifiable achievements or core projects matching the JD.
3. **Line 3 (The CTA):** Express interest and request resume exchange/evaluation (e.g., "方便交换简历聊聊吗？" or "方便发您一份简历评估吗？"). Do not claim the resume is already attached.

### Rule 4: Absolute Taboos 🚫
- **No System Defaults / Lazy Openings:** Never use auto-generated templates, "在吗" (Are you there?), or "还招人吗" (Still hiring?).
- **No Long Paragraphs:** Keep it under 4 lines. HR reading patience on mobile is very low.
- **No Age-Exposing Openings:** Do not start hooks with long work years (e.g., "14年经验..."); use professional titles or core competencies instead.

### Rule 5: JD Alignment & Handling Gaps 🎯
- **Direct Match:** Map target JD keywords and core requirements to matching facts in the user's resume.
- **Handling Gaps:** If the JD requires skills not on the resume, do not fabricate them. Highlight transferable skills or adjacent experience.
- **Quantifiable Output:** Focus on concrete outputs (latency, efficiency, revenue, users) to show capability, especially for low or partial matches.

---

## 🛠️ Execution & Output Format

When triggered:
1. **Read Resume:** Locate `resume.md` or ask the user to provide their background.
2. **Analyze JD:** Extract key requirements and pain points.
3. **Generate 3 Distinct Options:**
   - **Option 1 (Metric/Achievement-focused):** Focus on quantifiable data.
   - **Option 2 (Core Skill/Competency-focused):** Focus on core skills matching the JD.
   - **Option 3 (Background/Problem-solving focused):** Focus on matching background or solving a specific JD pain point.
4. **Output Format:** Provide only clean, send-ready text. Do NOT prefix lines with helper labels (e.g., "[Line 1]"). Keep the final output copy-paste ready.

### Example Output:
> **Option 1: Data-Driven Focus**
> 5年跨境产品经理，
> 曾主导XX系统搭建，实现订单转化率提升25%，获XX奖项。
> 仔细阅读了贵司JD，非常契合。方便交换简历聊聊吗？