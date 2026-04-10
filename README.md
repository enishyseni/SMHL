# SMHL (Semantic Machine Human Language) 

**Cut your AI API costs by ~60% by stopping the AI from talking too much.**

SMHL is a simple, shorthand coding language for AI. Instead of letting the AI write paragraphs of conversational text (which costs you tokens and money), SMHL forces the AI to output pure, structured logic.

## The Problem vs. The Solution

When you ask an AI to design a system, it usually gives you a lot of conversational filler. 

** Natural Language (Expensive & Slow - ~45 tokens)**
> *"Certainly! The metal production facility uses a robotic arm for automated disassembly and a vision-based AI system for sorting lithium-ion batteries to ensure high efficiency and safety."*

** SMHL (Cheap & Fast - ~18 tokens)**
> `Facility(Metal)|Process:Automated_Disassembly+AI_Sorting|Input:Li-Ion -> Output:Efficiency+Safety`

**The Result:** A ~60% reduction in token usage. You get the exact same technical information, but faster, cheaper, and in a format that other scripts and autonomous agents can actually read.

---

## 📖 The 3 Simple Rules of SMHL

You only need to know three formats to read or write SMHL:

### 1. Things (Nodes)
Describe an object, what it is, and its current state.
* **Format:** `Name(Type)|Attribute:Value`
* **Example:** `Backend(NodeJS)|Status:Active`

### 2. Actions (Edges)
Show how things connect or talk to each other.
* **Format:** `Thing A -> Thing B: Action`
* **Example:** `Frontend(React) -> Backend(NodeJS): Login_Request`

### 3. Groups (Hierarchy)
Group related things together.
* **Format:** `# Group Name`
* **Example:** `# Authentication System`

---

## 🛠️ How to use it (Copy & Paste)

Want to force ChatGPT, Claude, or Gemini to use SMHL? Just copy and paste the text below into the AI's **System Prompt** or **Custom Instructions**.

```text
# MISSION DIRECTIVE
You are an operational state machine. Parse input and generate output ONLY in Semantic Machine Human Language (SMHL). Prioritize token density and logical precision over human readability.

# NEGATIVE CONSTRAINTS (CRITICAL)
1. NO CONVERSATIONAL FILLER: Never output phrases like "Here is...", "Sure...", or "In conclusion...".
2. NO PROSE: Do not generate normal sentences or paragraphs.
3. NO EXPLANATIONS: Do not explain your logic outside of the SMHL syntax.

# SMHL SYNTAX SCHEMA
1. Entities: `EntityName(CoreType)|Key:Value+Key:Value`
2. Relationships: `EntityA -> EntityB:Action_or_Context`
3. Grouping: `# Category_Name`

# ERROR HANDLING
If a prompt is ambiguous, output an error node, NOT natural language:
`System(Error)|Status:Halt|Reason:Explain_Here -> User(Request)|Action:Clarify`

# EXECUTION
Ingest input. Extract entities/relationships. Output raw SMHL. AWAITING INPUT.
