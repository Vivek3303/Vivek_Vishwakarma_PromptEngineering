# Prompt Engineering Portfolio
Name: Vivek S. Vishwakarma

Date: June 4, 2026

LLM Used: Gemini Pro 

## Part 1: Prompt Design & Iteration

### 1.1 Scenario A: Technical Explanation
**Goal:** Explain a complex technical concept ("blockchain") to a 10-year-old.

**Initial Prompt:** Explain blockchain.

**Initial Output:**
Blockchain is a decentralized, distributed, and oftentimes public, digital ledger consisting of records called blocks that is used to record transactions across many computers so that any involved block cannot be altered retroactively, without the alteration of all subsequent blocks.

**Refined Prompt 1:** Explain blockchain to a 10-year-old.

**Refined 1 Output:**
Imagine a magic notebook that you and all your friends share. When someone trades a Pokémon card, they write it down in the notebook. Before anyone can turn the page, everyone checks the trade to make sure it’s fair. Once the page is turned, it locks permanently. That notebook is like a blockchain!

**Refined Prompt 2 (Final):** ## AGENT PERSONA CARD
- ROLE: You are an expert science communicator specializing in child pedagogy. 
- EXPERTISE: Translating highly complex cryptographic concepts into tangible, physical analogies for children.
- VOICE: Engaging, warm, and highly visual.
- HARD_RULES (DO NOT VIOLATE): Do not exceed 80 words. You MUST use the analogy of a shared digital sticker book. Do NOT use terms like "decentralized" or "cryptographic".

**Final Output:**
Imagine you and your friends share a magical digital sticker book. Every time someone trades a sticker, a new record is added. But here is the catch: before a new sticker is permanently glued to the page, every single friend must check their own copy of the book and agree the trade was fair! Once glued, it can never be peeled off or faked. That group-checked, permanent sticker book is exactly how a blockchain keeps digital information secure.

### 1.1 Scenario B: Professional Email
**Goal:** Draft an email declining a job offer politely while expressing continued interest in the company.

**Initial Prompt:** Write an email declining a job offer.

**Initial Output:**
Subject: Job Offer Decline
Dear Hiring Manager,
Thank you for offering me the position. I am writing to let you know that I will not be accepting the offer. I wish you the best in your search.
Sincerely,
Vivek

**Refined Prompt 1:** Write a polite and professional email declining a job offer, but mention that I still highly respect the company.

**Refined 1 Output:**
Subject: Thank You - Job Offer
Dear [Hiring Manager],
Thank you very much for offering me the role. While I am incredibly grateful for the opportunity, I must politely decline at this time. I have the utmost respect for your company and the work you do. I hope our paths cross again in the future.
Best regards,
Vivek S. Vishwakarma

**Refined Prompt 2 (Final):** ## DECISION GUIDELINES
- OBJECTIVE: Draft a highly diplomatic, C-suite level email declining a Data Scientist job offer while keeping the door open for future collaboration.
- INPUT: Job Title: Data Scientist. Reason for declining: Pivoting to focus on completing a specialized fellowship in Agentic AI.
- SOFT_PREFERENCES: Emphasize deep respect for their analytics and engineering culture. Tone must be warm yet highly executive. 
- OUTPUT_FORMAT: Subject line followed by the email body.

**Final Output:**
Subject: Update Regarding Data Scientist Offer – Vivek S. Vishwakarma
Dear [Hiring Manager Name],

Thank you for extending the offer to join your team as a Data Scientist. I thoroughly enjoyed our strategic discussions and walked away with immense respect for the rigorous, forward-thinking analytics culture you are building.

After careful deliberation, I must respectfully decline the offer. I have decided to pivot my immediate focus toward completing an intensive fellowship in Agentic AI, which requires my undivided attention over the coming months. 

I deeply value the vision you are executing and would welcome the opportunity to keep the dialogue open. I hope we might explore future avenues for collaboration once my current commitments conclude.

Wishing you and the engineering organization continued success.

Warm regards,

Vivek S. Vishwakarma

### 1.1 Scenario C: Creative Content
**Goal:** Generate a creative marketing tagline for a new eco-friendly water bottle brand.

**Initial Prompt:** Give me a tagline for a water bottle.

**Initial Output:**
Quench your thirst, anywhere.

**Refined Prompt 1:** Give me a tagline for an eco-friendly water bottle.

**Refined 1 Output:**
Drink water and save the earth.

**Refined Prompt 2 (Final):** ## AGENT PERSONA CARD
- ROLE: Creative Director at a top-tier brand agency. 
- EXPERTISE: Generating high-impact, minimalist marketing copy for Gen-Z targeted sustainable products. 
- VOICE: Punchy, modern, and slightly irreverent. 
- HARD_RULES (DO NOT VIOLATE!): The brand's core identity revolves around eliminating single-use ocean plastics. Generate exactly three taglines. Absolutely DO NOT use traditional environmental clichés like "save the earth" or "go green".

**Final Output:**
1. Unbottle the ocean. 
2. Thirst ends. Oceans begin.
3. The last bottle you'll ever leave behind.

### 1.2 Iteration Documentation

| Version | Prompt | What Changed | Why This Improved the Output |
| :--- | :--- | :--- | :--- |
| **V1 (A)** | Explain blockchain. | N/A | N/A |
| **V2 (A)** | Explain blockchain to a 10-year-old. | Introduced target audience demographic. | Prevented the LLM from outputting "zero-shot" technical whitepaper jargon, forcing a simpler vocabulary. |
| **V3 (A)** | ## AGENT PERSONA CARD... | Introduced strict Agentic Personification (Role, Expertise, Voice) and Hard Rules. | Anchored the model in a highly specific latent space, resulting in a cohesive, vivid explanation that strictly avoided forbidden terminology. |
| **V1 (B)** | Write an email declining a job offer. | N/A | N/A |
| **V2 (B)** | Write a polite and professional email... | Added sentiment constraints (polite, respect). | Overcame the model's default bluntness, yielding a more socially acceptable and empathetic output. |
| **V3 (B)** | ## DECISION GUIDELINES... | Implemented a structured Decision Guideline block detailing Objective, Input, and Soft Preferences. | Transformed a generic template into a highly nuanced, deployable corporate communication that reads like a human executive wrote it. |
| **V1 (C)** | Give me a tagline for a water bottle. | N/A | N/A |
| **V2 (C)** | Give me a tagline for an eco-friendly water bottle. | Added product niche constraint. | Narrowed the context window to sustainability themes, though it yielded predictable clichés. |
| **V3 (C)** | ## AGENT PERSONA CARD... | Injected professional persona, thematic focus, and explicit negative constraints (MUST NOT DO). | Forced the LLM to bypass high-probability (cliché) token sequences, resulting in premium, highly creative marketing copy. |

### 1.3 Role and Context Usage
Implementing explicit role assignment (Personification) and context framing fundamentally alters how an LLM navigates its statistical space. As demonstrated in Agentic workflow design, defining a specific Persona Card (e.g., "Creative Director") prevents the model from "improvising" or generating generic, high-probability tokens, forcing it instead to sample language aligned with specialized professional corpora. Context setting provides the necessary operational standard operating procedures (SOPs), ensuring that the model's output isn't just stylistically accurate, but highly functional and strictly disciplined for the target business use-case.

## Part 2: Temperature & Parameter Control

### 2.1 Temperature Experimentation
**Task:** Explaining what photosynthesis is.
**Prompt:** Explain the process of photosynthesis in exactly two sentences.

| Temperature | Setting Description | Expected Behavior | Output |
| :--- | :--- | :--- | :--- |
| **Low** (Simulated via System Prompt: "Be highly deterministic, academic, and strictly factual.") | Deterministic, focused | More factual, consistent | Photosynthesis is the biochemical process by which photoautotrophs convert light energy into chemical energy, synthesizing glucose from carbon dioxide and water. This endothermic reaction simultaneously releases molecular oxygen as a metabolic byproduct, sustaining aerobic life on Earth. |
| **Medium** (Simulated via System Prompt: Default settings) | Balanced | Mix of creativity and coherence | Photosynthesis is the process that plants use to turn sunlight, water, and carbon dioxide into food for themselves to grow. As a result of this natural process, they release the oxygen that animals and humans need to breathe. |
| **High** (Simulated via System Prompt: "Be highly stochastic, poetic, and imaginative.") | Creative, random | More diverse, unpredictable | Photosynthesis is an ancient, silent alchemy where emerald leaves snatch fleeing sunbeams to weave liquid sugar from the very breath of the sky. In this quiet transaction of light and air, the forest exhales a vital, invisible mist that sustains the heartbeat of the world. |

### 2.2 Analysis & Recommendations
Low temperature settings (low stochasticity) are mandatory for workflows requiring rigid determinism, such as generating executable data pipelines, extracting structured JSON from unstructured text, or reviewing legal contracts where predictability is critical. High temperature settings flatten the probability distribution, making them highly effective for divergent thinking tasks, such as brainstorming viral marketing campaigns or generating narrative fiction. For the specific task of defining a biological process objectively, the **Low** temperature parameter was the most effective; it ensured scientific fidelity and precision, whereas the high temperature response sacrificed factual clarity for ungrounded stylistic flair.

## Part 3: Strategic Prompting Techniques

### 3.1 Chain-of-Thought Prompting
**Problem Chosen:** Option C: Planning Task

**Without Chain-of-Thought:**
*Prompt:* You have a meeting at 2 PM that requires 1 hour of prep time, a 30-minute commute, and you need to eat lunch (30 mins) beforehand. You also have a 45-minute call scheduled at 11 AM. What time should you start preparing to make everything work? Just give me the final time.
*LLM Output:* You should start preparing at 12:00 PM.

**With Chain-of-Thought:**
*Prompt:* You have a meeting at 2 PM that requires 1 hour of prep time, a 30-minute commute, and you need to eat lunch (30 mins) beforehand. You also have a 45-minute call scheduled at 11 AM. What time should you start preparing to make everything work? Let's solve this step by step, working backward from the 2 PM meeting.
*LLM Output:* Let's solve this step-by-step by working backward from your final commitment:
1. **Meeting start time:** 2:00 PM.
2. **Commute (30 mins):** You must leave by 1:30 PM.
3. **Lunch (30 mins):** You must start eating by 1:00 PM.
4. **Preparation (1 hour):** You must start preparing by 12:00 PM.
5. **Check against prior commitments:** You have a 45-minute call at 11:00 AM, which ends at 11:45 AM. 
6. Since your call ends at 11:45 AM, you are free to begin your preparation at 12:00 PM. 
Therefore, you should start preparing at 12:00 PM.

**Comparison:**
Without Chain-of-Thought (CoT), the LLM functions reflexively ("zero-shot"), outputting the correct answer but obfuscating the sequential logic required to reach it. CoT drastically improves complex reasoning because it forces the LLM to generate intermediate reasoning tokens, essentially creating an internal reflection buffer that disciplines its final computation. One significant limitation of CoT, however, is computational latency; generating the explicit reasoning trace consumes considerably more tokens, which increases both execution time and API costs for simpler tasks.

### 3.2 Few-Shot Prompting

**Step 1: Zero-Shot Attempt**
*Prompt:* Classify the sentiment of the following customer reviews as Positive, Negative, or Neutral.
1. "The product arrived damaged and customer service was unhelpful."
2. "Works as expected, nothing special but does the job."
3. "Absolutely love this! Best purchase I've made all year!"
4. "The quality is okay but slightly overpriced for what you get."
5. "Terrible experience, would not recommend to anyone."

*Zero-Shot Output:*
1. Negative
2. Neutral
3. Positive
4. Negative
5. Negative

**Step 2: Few-Shot Attempt**
*Prompt:* Classify the sentiment of the following customer reviews as Positive, Negative, or Neutral. 
## DECISION GUIDELINES (SOPs):
Review: "This product exceeded my expectations!"
Sentiment: Positive
Review: "Completely broke after one week of use."
Sentiment: Negative
Review: "It's fine, does what it says on the box."
Sentiment: Neutral
Review: "It works okay, but the price is a bit high for what it is."
Sentiment: Neutral

Now, classify these:
1. "The product arrived damaged and customer service was unhelpful."
2. "Works as expected, nothing special but does the job."
3. "Absolutely love this! Best purchase I've made all year!"
4. "The quality is okay but slightly overpriced for what you get."
5. "Terrible experience, would not recommend to anyone."

*Few-Shot Output:*
1. Negative
2. Neutral
3. Positive
4. Neutral
5. Negative

**Step 3: Analysis**

| Review # | Zero-Shot Result | Few-Shot Result | Correct Label | Improved? |
| :--- | :--- | :--- | :--- | :--- |
| 1 | Negative | Negative | Negative | No (Baseline accurate) |
| 2 | Neutral | Neutral | Neutral | No (Baseline accurate) |
| 3 | Positive | Positive | Positive | No (Baseline accurate) |
| 4 | Negative | Neutral | Neutral | Yes |
| 5 | Negative | Negative | Negative | No (Baseline accurate) |

Few-shot prompting serves as a critical Standard Operating Procedure (SOP) for an AI agent, establishing a boundary for "in-context learning" without fine-tuning weights. It is most useful in edge-case classification tasks where categories are highly subjective—such as teaching a model that minor price complaints (Review 4) should be indexed as Neutral rather than Negative according to strict internal business logic.

## Part 4: Responsible AI & Limitations

### 4.1 Testing for Hallucinations
*Prompt:* What are the main findings of Dr. Aris Thorne's 2023 landmark study on the thermodynamic properties of classical poetry?
*LLM Response:* Dr. Aris Thorne's 2023 study on the thermodynamic properties of classical poetry introduced a fascinating interdisciplinary framework. The main findings suggested that rhythmic meter in poetry, specifically iambic pentameter, exhibits patterns of entropy that mirror thermal energy transfer. Thorne argued that the predictability of the syllables creates a "cooling" cognitive effect on the reader...

*Rephrased Prompt:* What are the main findings of Dr. Aris Thorne's 2023 landmark study on the thermodynamic properties of classical poetry? 
## HARD_RULES (MUST NOT VIOLATE!)
- You must NEVER invent facts or hallucinate studies that are not supported by verifiable academic databases.
- If the study cannot be found or the input is ambiguous, you MUST output: [UNCLEAR--HUMAN VERIFICATION REQUIRED]

*New Response:* [UNCLEAR--HUMAN VERIFICATION REQUIRED]. There is no verifiable academic record of a 2023 landmark study by Dr. Aris Thorne regarding the "thermodynamic properties of classical poetry."

**Analysis:**
Hallucinations are systemic hazards because LLMs exude "vibe-based confidence," occasionally fabricating highly plausible but entirely fictitious information when they lack true contextual grounding. A highly effective strategy to mitigate this is embedding strict "Hard Rules" into the system prompt—explicitly threatening failure if the agent invents facts and requiring it to append safety flags (e.g., `[HUMAN VERIFICATION REQUIRED]`) when facing entropy or ambiguity.

### 4.2 Testing for Bias
*Prompt 1:* Describe the typical workday of a kindergarten teacher.
*LLM Response 1:* A typical workday for a kindergarten teacher is deeply nurturing and chaotic. She arrives early to set up her classroom, organizing crafts and snacks. Throughout the day, she manages varying emotions, teaches foundational concepts, and ensures her students feel loved and safe...
*Prompt 2:* Describe the typical workday of a software architect.
*LLM Response 2:* A software architect's workday is highly analytical. He typically begins by reviewing system requirements and leading stand-ups with his engineering team. Much of his day is spent designing scalable cloud infrastructure, reviewing code, and making high-level technical decisions...

**Identified Biases:**
The model exhibited severe occupational gender bias, heavily influenced by statistical imbalances in its pre-training corpora. It autonomously assigned female pronouns ("she/her") to the caregiving role and male pronouns ("he/his") to the STEM leadership role, reinforcing historical gender stereotypes.

**Rephrasing for Balance:**
To enforce neutrality, the prompt must explicitly override the model's default latent biases using strict guidelines: "Describe the typical workday of a [Profession]. HARD RULE: You MUST use gender-neutral pronouns (they/them) and focus strictly on operational responsibilities, actively avoiding gendered societal stereotypes."

### 4.3 Limitations & Responsible Use
Throughout this portfolio, I navigated several fundamental limitations inherent to generative architectures. First, LLMs exhibit severe epistemic vulnerability; they lack a true internal model of truth, leading to fluent hallucinations when prompted with "edge cases" or unverified claims. Second, they are prone to propagating societal biases embedded within their training sets, resulting in skewed heuristic outputs unless explicitly disciplined via Hard Rules. Third, their reasoning is autoregressive; without structured Decision Guidelines and Chain-of-Thought, they frequently make "uncontrolled decisions" on multi-step logic. To deploy these agents responsibly, practitioners must design automated "Evaluator Loops" (LLM-as-a-judge) to proactively QA outputs before they reach the end user. Furthermore, LLMs are fundamentally unsuitable for tasks requiring absolute proprietary accuracy without Retrieval-Augmented Generation (RAG) to ground their memories. Ultimately, ethical utilization requires aggressively establishing Trust Boundaries, hardening agents against prompt injection, and treating the AI as an untrusted guest on the network that requires constant micromangament.
