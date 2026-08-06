# AI Research & Prompt Engineering — Study Notes

> Prep notes for AI Research & Prompt Engineering role (WeGro). Covers: AI platform comparison, prompt engineering, model strengths/limits, business use cases, and role fundamentals.

---

## Table of Contents

1. [Comparing Major AI Platforms](#1-comparing-major-ai-platforms)
2. [Prompt Engineering Techniques & System Instructions](#2-prompt-engineering-techniques--system-instructions)
3. [Real Strengths & Limits of Current AI Models](#3-real-strengths--limits-of-current-ai-models)
4. [Practical Business Use Cases for AI](#4-practical-business-use-cases-for-ai)
5. [Fundamentals of the Role: AI Research & Prompt Engineering](#5-fundamentals-of-the-role-ai-research--prompt-engineering)
6. [Quick Reference / One-Liners](#6-quick-reference--one-liners)

---

## 1. Comparing Major AI Platforms

Test questions in this area care about **when you'd choose each tool**, not just definitions.

| AI Platform    | Best For                                  | Strengths                                                                        | Limitations                                                         |
| -------------- | ------------------------------------------ | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| **ChatGPT**    | Writing, coding, brainstorming, learning  | Versatile, strong coding support, good explanations                              | Can still make mistakes or confidently state incorrect information |
| **Claude**     | Long documents, careful writing, analysis | Excellent with long text, natural writing style, strong summarization            | Not the best choice for every coding or web-based task              |
| **Gemini**     | Google ecosystem, multimodal tasks        | Integrates well with Google services, handles text, images, and more             | Performance varies depending on the task and model version          |
| **Perplexity** | Research and web search                   | Searches the web and usually cites sources, good for finding recent information  | Less suited to long creative writing or complex document drafting   |

### When to use each

- **Write a report / debug code?** → ChatGPT
- **Summarize a 100-page PDF?** → Claude
- **Work in Google Docs / Gmail / Workspace?** → Gemini
- **Need the latest info with sources?** → Perplexity

### Scenario-based practice

| Scenario | Answer |
|---|---|
| Research latest AI regulations, cite reliable sources | **Perplexity** |
| Summarize a very long contract | **Claude** |
| Write and debug SQL queries | **ChatGPT** |
| Team working in Google's ecosystem wants integrated AI | **Gemini** |

> Exams are more likely to ask scenario questions ("A manager needs X, which tool?") than plain definitions.

### MCQ Practice

**1. Which AI tool is generally best for finding recent information with cited sources?**
A. ChatGPT B. Claude C. Gemini D. Perplexity
✅ **D. Perplexity**

**2. Which AI is especially known for handling long documents and detailed summaries well?**
A. Claude B. Perplexity C. Gemini D. None
✅ **A. Claude**

**3. Best choice for writing Python code and explaining algorithms?**
A. ChatGPT B. Perplexity C. Calculator D. Browser
✅ **A. ChatGPT**

---

## 2. Prompt Engineering Techniques & System Instructions

### 2.1 What is Prompt Engineering?

A **prompt** = the instruction/question given to an AI.

- ❌ Weak: `"Write an email."`
- ✅ Strong: `"You are an HR manager. Write a professional interview invitation email in under 150 words with a friendly tone."`

**Prompt engineering** = the skill of writing prompts that produce better, more useful AI output.

### 2.2 Core Techniques

**A. Role Prompting** — tell the AI who to act as
> "Act as a software engineer." / "You are a marketing expert."

**B. Give Context** — provide background info
- ❌ `Write a report.`
- ✅ `Write a report on the benefits of AI for a startup in Bangladesh.`

**C. Set Constraints** — define limits
- Under 200 words
- Use bullet points
- Explain in simple English
- Don't use technical jargon

**D. Specify Output Format**
- ❌ `Compare ChatGPT and Claude.`
- ✅ `Compare ChatGPT and Claude in a table with columns for strengths, weaknesses, and best use cases.`

**E. Zero-shot / One-shot / Few-shot**

| Type | Meaning | Example |
|---|---|---|
| Zero-shot | Task only, no examples | "Translate this sentence into Bengali." |
| One-shot | One example given first | "Cat → Animal, Dog → ?" |
| Few-shot | Several examples given before the task | Multiple pattern examples, then continue |

### 2.3 System Instructions vs. User Prompts

- **System instruction** — sets the AI's overall behavior/role for the whole conversation.
  > "You are a helpful AI tutor. Explain everything in simple language."
- **User prompt** — the specific request made in the conversation.
  > "Explain percentages."

> System instruction = sets the **role**. User prompt = sets the **task**.

### 2.4 Note on Chain-of-Thought

"Chain-of-thought prompting" is a well-known concept, but **not every model reveals its internal reasoning**. For exams/practical use: focus on asking the model to *explain its answer* or *show its working*, rather than expecting raw internal reasoning access.

### MCQ Practice

**1. What is prompt engineering?**
A. Building robots B. Writing effective prompts to get better AI responses C. Training neural networks D. Creating websites
✅ **B**

**2. Which technique asks the AI to behave as a specific expert?**
A. Role prompting B. Random prompting C. Numeric prompting D. Image prompting
✅ **A**

**3. What is the purpose of a system instruction?**
A. To change the AI's overall behavior or role B. To install software C. To connect to the internet D. To increase computer memory
✅ **A**

---

## 3. Real Strengths & Limits of Current AI Models

### ✅ Strengths

| Area | Examples |
|---|---|
| **Writing** | Emails, reports, blogs, social posts |
| **Summarization** | Long documents, PDFs, meeting notes, research papers |
| **Coding Assistance** | Writing code, debugging, explaining code, test cases |
| **Brainstorming** | Business ideas, marketing campaigns, product names |
| **Translation** | English ↔ Bangla, and many other languages |
| **Learning & Explaining** | Simplifying concepts, study notes, Q&A |
| **Data Analysis** | Finding patterns, summarizing data, reports (tool-dependent) |

### ❌ Limitations

1. **Hallucinations** ⭐⭐⭐ — confident but incorrect answers; may invent facts, quotes, or references.
2. **No Human Understanding** — no emotions/consciousness; predicts likely text from patterns.
3. **Can Misunderstand Vague Prompts** — e.g. `"Write something."` gives poor results; clarity matters.
4. **Bias** — can reflect biases present in training data.
5. **Privacy** — avoid pasting confidential company data, passwords, or sensitive personal info into public AI tools.
6. **Knowledge Limitations** — may not know recent events without live web access.
7. **Needs Human Verification** — important legal, medical, financial, or business decisions should always be human-reviewed.

### MCQ Practice

**1. Which is a major limitation of current AI models?**
A. They never make mistakes B. They can confidently provide incorrect information C. They don't understand English D. They cannot write emails
✅ **B**

**2. Which task is AI generally good at?**
A. Summarizing long documents B. Predicting the future with certainty C. Never making factual mistakes D. Replacing all human judgment
✅ **A**

**3. Why should businesses verify AI-generated content?**
A. AI can produce inaccurate or fabricated information B. AI refuses to answer C. AI cannot generate text D. AI always asks for payment
✅ **A**

> 💡 **Key sentence:** Current AI models excel at generating, summarizing, explaining, and brainstorming — but can make factual mistakes, reflect bias, and shouldn't be trusted blindly for important decisions.

---

## 4. Practical Business Use Cases for AI

Core question: **"How can a company actually use AI in daily work?"** — think beyond content generation; focus on speed, efficiency, and smarter workflows.

| Department | Example Uses |
|---|---|
| **Customer Support** | Draft replies to common questions, generate FAQs, respond to order queries |
| **Marketing** | Social media posts, ad copy, campaign ideas, analyze customer feedback |
| **HR** | Draft job descriptions, screen CVs (with human review), interview questions, onboarding docs |
| **Finance** | Summarize financial reports, explain spreadsheets, draft budget summaries, flag unusual spending |
| **Research** | Summarize articles, compare competitors, track industry trends, prep research notes |
| **Operations** | Create SOPs, draft reports, organize info, summarize meetings |
| **Software Development** | Write/debug code, generate test cases, explain programming concepts |
| **Sales** | Sales emails, personalized customer messages, meeting summaries, proposals |

### WeGro-specific (agri-tech / agri-fintech) examples
- Summarize farmer feedback
- Draft investor update emails
- Analyze market trends
- Generate management reports
- Translate content (Bangla ↔ English)
- Answer common farmer/investor questions

### MCQ Practice

**1. Which department can benefit from AI?**
A. HR B. Finance C. Marketing D. **All of the above** ✅

**2. Which is a practical business use of AI?**
A. Customer support replies B. Summarizing reports C. Brainstorming marketing ideas D. **All of the above** ✅

**3. Why do companies use AI?**
A. Automate repetitive tasks B. Improve productivity C. Assist better decision-making D. **All of the above** ✅

### 🎯 Interview-style Q&A

**Q: How could WeGro use AI to improve its business?**
> "WeGro could use AI to summarize farmer and investor communications, draft emails and reports, support market research, analyze agricultural and financial data, generate marketing content, and help employees work more efficiently. Human staff would still review important decisions and communications."

---

## 5. Fundamentals of the Role: AI Research & Prompt Engineering

### 5.1 What is AI Research (in a business context)?

**Not** inventing new AI models. It means:
- Researching new AI tools
- Comparing different AI models
- Testing new AI features
- Finding the best tool for a business task
- Documenting findings

**Example:** Comparing ChatGPT, Claude, and Gemini for summarizing investor reports, then recommending:
> "Claude produced the clearest summaries for long reports, while ChatGPT was stronger at explaining technical concepts."

### 5.2 What is Prompt Engineering?

Designing and improving prompts so AI gives better answers.
- ❌ `Write an email.`
- ✅ `You are an HR manager. Write a professional interview invitation email in under 120 words with a friendly tone.`

### 5.3 Typical Responsibilities

| Category | Activities |
|---|---|
| **Research** | Test AI tools, compare results, track new features |
| **Experiment** | Try different prompts, measure effectiveness |
| **Documentation** | Write findings reports, record strengths/weaknesses |
| **Business Application** | Recommend departmental AI use cases |
| **Communication** | Explain AI clearly to non-technical stakeholders (incl. leadership) |

### 5.4 Skills Required

**Technical**
- Understand AI tools
- Write effective prompts
- Compare AI models
- Evaluate AI outputs

**Soft Skills**
- Communication
- Problem-solving
- Curiosity
- Critical thinking

### 5.5 Typical Workflow Example

CEO asks: *"Which AI should we use to summarize investor reports?"*

1. Test ChatGPT
2. Test Claude
3. Test Gemini
4. Compare quality, speed, ease of use
5. Recommend the best option
6. Provide example prompts

### MCQ Practice

**1. Main purpose of AI research in a company?**
A. Build robots B. **Compare AI tools and identify the best solution for business needs** ✅ C. Design computer chips D. Repair computers

**2. What is prompt engineering?**
A. **Writing effective prompts to improve AI output** ✅ B. Building websites C. Programming operating systems D. Installing AI software

**3. Which activity best matches an AI Research Intern?**
A. **Comparing Claude and ChatGPT for report summarization** ✅ B. Repairing office printers C. Installing Windows D. Managing payroll

### 5.6 Interview Prep

**Q: What do you think an AI Research & Prompt Engineering Intern does?**
> "An AI Research & Prompt Engineering Intern evaluates AI tools, compares their strengths and limitations, designs effective prompts, tests AI in real business scenarios, documents the results, and recommends how different departments can use AI to improve productivity."

**Likely follow-up interview questions:**
- Why is Claude better than ChatGPT for some tasks?
- How would you use AI in HR or finance?
- Show us how you'd improve a weak prompt.

---

## 6. Quick Reference / One-Liners

- **ChatGPT** → writing, coding, brainstorming
- **Claude** → long documents, careful writing/analysis
- **Gemini** → Google ecosystem, multimodal
- **Perplexity** → web research with citations
- **Prompt engineering** = role + context + constraints + format + examples (zero/one/few-shot)
- **System instruction** = sets role/behavior | **User prompt** = sets the task
- **Biggest AI risk** = hallucination (confident but wrong answers)
- **Golden rule** = AI assists, humans verify — especially for legal/medical/financial/business decisions
- **AI Research role** = compare tools, test prompts, document findings, recommend business applications

---
*Compiled study notes — ready for exam review and interview prep.*
