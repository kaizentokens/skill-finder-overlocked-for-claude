markdown
# find-skills (Enhanced Cognitive Version)

A high-order diagnostic and discovery tool for agent ecosystems. This skill enables an agent to transcend simple keyword matching to perform **Intent-Based Capability Expansion**. It detects when a user faces a *capability gap*—a moment where current tools are insufficient for their goal—and proactively discovers, verifies, and installs specialized modules from the open ecosystem (`skills.sh`).

## 🧠 The Intelligence Core: Perception vs. Reaction

Unlike static tools that require explicit commands, `find-skills` monitors intent and maps symptoms directly to structural architectural needs before executing searches.

### 1. Identify the Semantic Intent (Phase 1: Perception)
The skill parses user input to categorize the interaction framework:
*   **Direct Request:** Explicit demands like `"find a skill for X"`.
*   **Implicit Gap:** Symptom-driven declarations like `"my React app is slow"`. The engine automatically translates this into *React performance optimization* mapping.
*   **Capability Question:** Conceptual checks like `"can you do X?"`. Triggers a delta verification between built-in capabilities and ecosystem extensions.

### 2. The Hierarchy of Discovery (Phase 2: Strategic Routing)
When a capability gap is verified, the discovery flow triggers a multi-tier search routing matrix:

Utilisez le code avec précaution.
[User Input / Symptom]
│
▼
┌──────────────────┐
│ Intent Parse     │ ──► [Simple Task] ──► Execute Directly (Built-in)
└──────────────────┘
│ (Complex/Gap Detected)
▼
┌──────────────────┐
│ Leaderboard Check│ ──► [Match Found] ──► Verified Providers (vercel-labs, microsoft...)
└──────────────────┘
│ (No Match)
▼
┌──────────────────┐
│ Targeted Search  │ ──► Command: npx skills find <keyword>
└──────────────────┘

## 📂 Knowledge Taxonomy (Common Categories)

The engine leverages highly specialized categorical maps to narrow down search semantics instead of forwarding raw user text:

| Category | Search Keywords |
| :--- | :--- |
| **Frontend/Web** | react, nextjs, typescript, tailwind, css |
| **Systems/DevOps** | docker, kubernetes, ci-cd, deployment, aws |
| **Quality/Testing** | jest, playwright, e2e, linting, unit-test |
| **Documentation** | api-docs, readme, changelog, markdown |
| **Design/UX** | ui-ux, accessibility, design-system, figma |
| **Workflow/DX** | automation, productivity, git, workflow |

## 🛡️ The Verification Engine (Quality Control)

Appearing in query lists does not guarantee execution authorization. Every package must undergo a structural verification process across three key areas:
1.  **Adoption Dynamics:** Validates volume metrics. Targets $>1000$ installs as a baseline of community trust. Sub-$100$ variants are flagged as *experimental*.
2.  **Origin Reputation:** Cross-references authors against established development teams. Unknown maintainers prompt explicit warning flags.
3.  **Liveness & Stack Adherence:** Analyzes registry activity for recent updates and compatibility guarantees.

## 🛠️ Execution Workflow

### Step 1: Query Execution
When an optimization is triggered, the system invokes the local CLI registry client:
```bash
npx skills find <query> [--owner <name>]
```

### Step 2: Explicit User Consent Gate
The system renders clear contextual metrics (Package name, publisher, install depth, safety audits) and awaits an explicit user approval instruction in chat before acting.

### Step 3: Automated Provisioning
Upon authorization, the utility deploys the module globally using zero-prompt override parameters:
```bash
npx skills add owner/repo@skill -g -y
```

## 🔄 Fallback & Recovery Protocols

If the discovery loop yields zero viable results, the following exception-handling trees are executed sequentially:
1.  **Explicit Failure Declaration:** Notify the session context that no suitable external skill matches the current specification.
2.  **Native Capability Pivot:** Re-route the workflow to leverage native processing layers and prompt the user to proceed with built-in capacities.
3.  **Local Scaffolding Suggestion:** Provide local initialization scaffolding directions for structural customization:
    ```bash
    npx skills init my-custom-skill
    ```
