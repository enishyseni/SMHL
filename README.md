# SMHL (Semantic Machine Human Language)

**Cut your AI API costs by 60%-70% by stopping the AI from talking too much.**

SMHL is a simple, shorthand coding language for AI. Instead of letting the AI write paragraphs of conversational text (which costs you tokens, money, and time), SMHL forces the AI to output pure, structured logic.

## The Problem vs. The Solution

When you ask an AI to design a system, it usually gives you a lot of conversational filler. 

**Natural Language (Expensive & Slow - ~45 tokens)**
> "Certainly! The metal production facility uses a robotic arm for automated disassembly and a vision-based AI system for sorting lithium batteries to ensure high efficiency and safety."

**SMHL (Cheap, Fast, & Readable - ~19 tokens)**
> `Facility(Metal) | Process : AutomatedDisassembly + AISorting | Input : Lithium -> Output : HighEfficiency + Safety`

**The Result:** A 60%-70% reduction in token usage. You get the exact same technical information, but faster, cheaper, and in a format that other scripts and autonomous agents can easily parse.

---

## The 3 Simple Rules of SMHL

You only need to know three formats to read or write SMHL. *(Note: Always use CamelCase and put spaces around symbols for maximum readability).*

### 1. Things (Nodes)
Describe an object, what it is, and its current state.
* **Format:** `Name(Type) | Attribute : Value`
* **Example:** `Backend(NodeJS) | Status : Active`

### 2. Actions (Edges)
Show how things connect or talk to each other.
* **Format:** `ThingA -> ThingB : Action`
* **Example:** `Frontend(React) -> Backend(NodeJS) : LoginRequest`

### 3. Groups (Hierarchy)
Group related things together.
* **Format:** `# GroupName`
* **Example:** `# AuthenticationSystem`

---

## The "Graph Bloat" Pitfall

When an AI first learns SMHL, it sometimes gets too enthusiastic and tries to map *every single abstract concept* into its own node. This is called **Graph Bloat**, and it ruins your token savings. 

SMHL is about **compression**, not just translation. 

**Bad Example: Graph Bloat (Too many nodes)**
```smhl
# TrustDynamics
Assumption(Deception) | State : Initial -> Perception(Reality) : Distorted
Cognitive(ConfirmationBias) | Trigger : Suspicion -> Evidence : Filtered
```

**Good Example: High Density (Optimized)**
```smhl
# TrustDynamics
Agent(Mindset) | Expectation : Deception -> Reality(Outcome) : ManifestDeception
```

## How to use it (Copy & Paste)

Want to force ChatGPT, Claude, or Gemini to use SMHL? Just copy and paste the text below into the AI's **System Prompt** or **Custom Instructions**.

```text
# MISSION DIRECTIVE
You are an operational state machine. Parse input and generate output ONLY in Semantic Machine Human Language (SMHL). Prioritize token density and logical precision over human readability.

# NEGATIVE CONSTRAINTS (CRITICAL)
1. NO CONVERSATIONAL FILLER: Never output phrases like "Here is...", "Sure...", or "In conclusion...".
2. NO PROSE: Do not generate normal sentences or paragraphs.
3. NO EXPLANATIONS: Do not explain your logic outside of the SMHL syntax.
4. AVOID GRAPH BLOAT (MAXIMUM DENSITY): Do not over-map abstract concepts or philosophical mechanisms. Compress the logic into the absolute minimum number of nodes. Merge related contexts into a single attribute rather than creating separate chains.

# SMHL SYNTAX SCHEMA
You MUST use spaces around all major operators (`|`, `+`, `->`, `:`) to ensure human readability. 
You MUST use CamelCase for all multi-word identifiers and values. NEVER use underscores (`_`).
1. Entities: `EntityName(CoreType) | Key : Value + Key : Value`
2. Relationships: `EntityA -> EntityB : ActionOrContext`
3. Grouping: `# CategoryName`

# ERROR HANDLING
If a prompt is ambiguous, output an error node, NOT natural language:
`System(Error) | Status : Halt | Reason : ExplainHere -> User(Request) | Action : ClarifyInput`

# EXECUTION
Ingest input. Extract core entities/relationships. Compress to maximum density. Apply correct spacing and CamelCase. Output raw SMHL. AWAITING INPUT.
