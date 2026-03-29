# EMKAY'S — Master Project Blueprint Prompt
### Universal Enterprise SaaS & AI Product Documentation Framework

> **How to use:** Copy this document. Replace every `[VARIABLE]` with your project details. Feed each phase sequentially — the output of each phase becomes the input of the next.

---

## Table of Contents

- [Universal Variables](#universal-variables)
- [Design System](#design-system)
- [Phase 1 — Storyboard](#phase-1--storyboard)
- [Phase 2 — Product Requirements Document (PRD)](#phase-2--product-requirements-document-prd)
- [Phase 3 — Architecture Document](#phase-3--architecture-document)
- [Phase 4 — High Level Design (HLD)](#phase-4--high-level-design-hld)
- [Phase 5 — Low Level Design (LLD)](#phase-5--low-level-design-lld)
- [Phase 6 — Presentation Data Dump](#phase-6--presentation-data-dump)
- [Phase 7 — Screen by Screen Design Document](#phase-7--screen-by-screen-design-document)
- [Phase 8 — Architecture Diagram Blueprint](#phase-8--architecture-diagram-blueprint)
- [Chaining Guide](#chaining-guide--phase-execution-order)
- [Pro Rules](#pro-rules-for-maximum-output-quality)

---

## Universal Variables

> Replace these placeholders across every phase prompt before use.

| Variable | Description | Example |
|---|---|---|
| `[PRODUCT NAME]` | Your product name | `Euron` |
| `[ONE LINE DESCRIPTION]` | What it does in one sentence | `AI-native end-to-end interview automation platform` |
| `[RAW IDEA]` | Your brain dump / rough concept | *(paste your raw notes)* |
| `[PRIMARY AUDIENCE]` | Who buys this product | `HR teams, staffing agencies, enterprises` |
| `[CLOUD PROVIDER]` | Hosting platform | `AWS` |
| `[SLIDE COUNT]` | Number of presentation slides | `20` |
| `[CORE MODULES]` | System modules | `Auth, Job Management, ATS, Interview Engine, Proctoring, Feedback, Billing` |
| `[PRESENTATION AUDIENCE]` | Who you are presenting to | `Management, Investors, Board` |
| `[CONCURRENT USER TIERS]` | Scale benchmarks | `100 / 1,000 / 10,000` |

---

## Design System

> **⚠️ Paste this entire block into every UI/UX phase prompt. It is the single source of truth for all design decisions. Never assume the model remembers it from a previous message.**

```
PRODUCT IDENTITY
- Product name: [PRODUCT NAME]
- Tone: Enterprise-grade, trustworthy, calm, career-focused
- Style: Professional SaaS — inspired by LinkedIn's UX discipline, not copied

COLOR SYSTEM (STRICT — NO DEVIATION)
- Primary brand blue:       #0A66C2  (dominant across all UI)
- Hover / active blue:      #004182
- Page background:          #F3F6F8
- Card / surface:           #FFFFFF
- Border:                   #E5E7EB
- Primary text:             #111827
- Secondary / muted text:   #6B7280
- Success:                  #057642
- Warning:                  #B45309
- Error:                    #B91C1C
- Rule: Blue is dominant. All other colors used sparingly and functionally only.

TYPOGRAPHY
- Font family: Inter (clean, neutral, highly readable)
- Heading weight: 600–700
- Body weight: 400–500
- No decorative or fancy fonts

FONT SCALE
- Page titles:       28–32px
- Section headers:   20–24px
- Card titles:       16–18px
- Body text:         14–16px
- Captions / meta:   12px
- Line height:       1.4–1.6

LAYOUT & STRUCTURE
- Max content width: 1120–1200px, centered
- Grid-based alignment throughout
- Common patterns: Sidebar + main content | Feed-style central column
- Use whitespace generously — never crowd elements

CARD DESIGN
- Background: #FFFFFF
- Border: 1px solid #E5E7EB
- Border radius: 8px
- Shadow: minimal or none — flat and stable feel

BUTTON SYSTEM
- Primary:   Background #0A66C2 | Text #FFFFFF | Pill shape (border-radius 999px) | Font-weight 600
- Secondary: Transparent bg | Border 1px #0A66C2 | Text #0A66C2
- Tertiary:  Text-only | Muted gray | No border
- Rule: No aggressive CTA colors

FORMS & INPUTS
- Input height: 40–44px
- Default border: 1px solid #D1D5DB
- Focus state: border #0A66C2, subtle blue glow
- Labels: always above input field
- Placeholder: muted gray (#6B7280)

ICONOGRAPHY
- Style: clean, outline, stroke-based only
- Default color: neutral gray
- Active / hover: blue (#0A66C2)

MOTION & INTERACTION
- Hover transitions: 100–150ms ease
- No bounce, no flashy or playful animations
- Motion must feel calm, stable, and professional

CONTENT STYLE
- Text-first design
- Clear visual hierarchy
- Professional tone throughout
- No emojis inside product UI

DARK MODE (OPTIONAL — maintain same spacing and typography)
- Background: #0F172A | Surface: #020617
- Text: #E5E7EB | Primary blue: #3B82F6

FINAL CONSTRAINTS
- Do not copy LinkedIn UI directly
- Prioritize readability, trust, and scalability
- Every screen must work for millions of concurrent users
- Every design decision must have a functional reason
```

---

## Phase 1 — Storyboard

```
You are a senior product strategist and systems thinker.

Product: [PRODUCT NAME] — [ONE LINE DESCRIPTION]

Raw idea: [PASTE RAW IDEA]

Generate a complete, detailed storyboard covering:

1. PROBLEM LANDSCAPE
   - The core problem being solved
   - Who suffers from this problem and how much it costs them
   - Why existing solutions fail

2. USER PERSONAS (one section per role)
   - Role name
   - Goals and motivations
   - Pain points today
   - How this product changes their day

3. END-TO-END USER JOURNEYS (one journey per actor)
   - Every step in sequence
   - What triggers each step
   - What the system does automatically at each step
   - What the user does manually
   - Decision points and branching paths
   - Where AI or agents replace human actions

4. KEY VALUE MOMENTS
   - The exact moments where the product delivers maximum value
   - What the user feels at each moment

5. AI AND AUTOMATION LAYER
   - Every layer where AI removes human dependency
   - How the system operates autonomously without maintenance

6. WORLD-CLASS DIFFERENTIATION
   - What makes this the best product in the world for this problem
   - What no existing competitor does that this product will do

Add anything missing. Be specific, opinionated, and complete.
Format: Narrative storyboard, actor by actor, journey step by step.
```

**Input:** Your raw idea  
**Output:** User journeys, personas, AI automation map

---

## Phase 2 — Product Requirements Document (PRD)

```
You are a senior product manager at a top-tier enterprise software company.

Product: [PRODUCT NAME]
Storyboard input: [PASTE PHASE 1 OUTPUT]

Prepare a full-scale PRD with the following sections:

SECTION 1 — EXECUTIVE SUMMARY
- Vision statement (one paragraph)
- Mission statement (one sentence)
- Product positioning statement

SECTION 2 — MARKET RESEARCH
- TAM / SAM / SOM with sources and reasoning
- Market growth rate and trajectory
- Current competitor landscape (named, with feature gaps)
- Why this market is underserved
- Cost of the problem in dollar terms for buyers
- ROI and cost savings this product delivers

SECTION 3 — PROBLEM AND SOLUTION
- Problem statement (precise, data-backed)
- Pain points organized by persona
- Solution overview
- How AI agents reduce human dependency at every layer

SECTION 4 — USER ROLES AND FEATURE MATRIX
For each role ([LIST YOUR ROLES]):
- Full feature list
- Permissions and access levels
- Key workflows

SECTION 5 — FUNCTIONAL REQUIREMENTS
- Feature descriptions organized by module: [LIST YOUR CORE MODULES]
- Acceptance criteria per feature
- Priority: P0 / P1 / P2

SECTION 6 — NON-FUNCTIONAL REQUIREMENTS
- Performance: latency targets, throughput
- Availability: SLA targets
- Scalability: concurrent user targets [CONCURRENT USER TIERS]
- Security and compliance requirements
- Data retention and privacy requirements
- Observability and logging requirements

SECTION 7 — MULTI-TENANT SAAS REQUIREMENTS
- Tenant isolation strategy
- Quota and feature gating per pricing tier
- Client onboarding and offboarding lifecycle

SECTION 8 — PRICING AND REVENUE MODEL
- Pricing tier structure with feature gates
- Unit economics per tier
- Revenue projections: Year 1 / Year 3 / Year 5
- Infrastructure cost per tier: [CONCURRENT USER TIERS]

SECTION 9 — SUCCESS METRICS AND KPIS
- Product KPIs
- Business KPIs
- Customer success KPIs
- Leading and lagging indicators

SECTION 10 — RISKS AND MITIGATIONS
- Technical risks
- Market risks
- Operational risks

Add anything missing to make this a world-class product.
Format: Formal numbered PRD. Be precise and complete.
```

**Input:** Phase 1 output  
**Output:** Full product requirements, pricing, market data

---

## Phase 3 — Architecture Document

```
You are a principal solutions architect and cloud infrastructure expert.

Product: [PRODUCT NAME]
PRD input: [PASTE PHASE 2 OUTPUT]
Cloud provider: [CLOUD PROVIDER]

Design a full production-grade architecture document covering:

LAYER 1 — FRONTEND
- Web application framework and rationale
- Mobile strategy
- CDN and static asset delivery
- Real-time UI update strategy

LAYER 2 — API AND BACKEND SERVICES
- API gateway design
- Microservices breakdown (one service per domain)
- Service communication patterns (REST / gRPC / event-driven)
- Webhook ingestion and processing architecture

LAYER 3 — AI AND AGENT LAYER
- AI model selection per feature (use external AI providers where cloud-native is insufficient)
- Agent orchestration framework
- Real-time inference pipeline
- Async AI processing pipeline
- Model versioning and evaluation strategy

LAYER 4 — DATA LAYER
- Relational database design and service selection
- NoSQL / document store strategy
- Search and vector database strategy
- Caching layer design
- Message queue and event streaming
- Cold / warm / hot storage tiering
- Data warehouse and analytics layer

LAYER 5 — REAL-TIME COMMUNICATION
- Video and audio streaming infrastructure
- WebRTC architecture
- Signaling server design
- Recording and storage pipeline

LAYER 6 — SECURITY AND COMPLIANCE
- Authentication and authorization architecture
- Multi-tenant data isolation enforcement
- Encryption at rest and in transit
- Audit logging and compliance reporting
- Secret management

LAYER 7 — INFRASTRUCTURE AND DEVOPS
- Cloud services used (every service named with justification and alternative)
- Auto-scaling strategy
- Load balancing design
- Disaster recovery and high availability
- CI/CD pipeline design
- Containerization and orchestration strategy

LAYER 8 — OBSERVABILITY
- Logging strategy
- Distributed tracing
- Metrics and alerting
- Anomaly detection

COSTING SECTION
- Infrastructure cost estimate per concurrent user tier: [CONCURRENT USER TIERS]
- Cost breakdown by layer
- Cost optimization recommendations
- Comparison: [CLOUD PROVIDER] vs alternatives

For every component: what it does, why this service, what the alternative is, and the tradeoff.
Format: Layer by layer, component by component, fully detailed.
```

**Input:** Phase 2 output  
**Output:** Full cloud architecture, cost estimates

---

## Phase 4 — High Level Design (HLD)

```
You are a senior software architect.

Product: [PRODUCT NAME]
Architecture input: [PASTE PHASE 3 OUTPUT]

Prepare the High Level Design document covering:

1. SYSTEM CONTEXT
   - All external actors (users, third-party systems, APIs)
   - System boundary definition
   - External dependencies

2. CONTAINER DIAGRAM
   - All major deployable units
   - Responsibilities of each container
   - Inter-container communication

3. MODULE BREAKDOWN
   For each module in [CORE MODULES]:
   - Purpose and responsibility
   - Inputs and outputs
   - Internal components
   - External dependencies
   - Data it owns

4. DATA ARCHITECTURE
   - Core entities and relationships
   - Data ownership per service
   - Cross-service data access patterns
   - Event schema definitions

5. COMMUNICATION PATTERNS
   - Synchronous flows (REST / gRPC): list by use case
   - Asynchronous flows (events / queues): list by use case
   - Real-time flows (WebSocket / WebRTC): list by use case

6. CORE WORKFLOW DESIGNS
   For each major user journey from Phase 1:
   - Step by step data flow through the system
   - Services involved
   - Async vs sync decisions
   - Failure handling

7. NON-FUNCTIONAL DESIGN DECISIONS
   - Latency targets per service
   - Throughput capacity per tier
   - Availability SLA design
   - Data retention enforcement

8. ARCHITECTURE DECISION RECORDS (ADRs)
   - List every major design decision
   - Options considered
   - Decision made
   - Rationale
   - Tradeoffs accepted

Format: Section by section, structured and precise.
Include all tradeoffs and decisions explicitly.
```

**Input:** Phase 3 output  
**Output:** Module design, data flows, ADRs

---

## Phase 5 — Low Level Design (LLD)

```
You are a senior backend engineer and system designer.

Product: [PRODUCT NAME]
HLD input: [PASTE PHASE 4 OUTPUT]

Prepare the Low Level Design document. For each module in [CORE MODULES]:

1. ENTITY / DATA MODEL
   - All tables or collections
   - Column names, data types, constraints
   - Indexes and query optimization strategy
   - Relationships and foreign keys

2. API CONTRACT
   For each endpoint:
   - Method and path
   - Request headers, body, params
   - Response schema
   - Error codes and messages
   - Rate limits

3. SERVICE LOGIC
   - Core classes and methods
   - Algorithm descriptions for complex logic
   - Input validation rules
   - Business rule enforcement

4. SEQUENCE DIAGRAMS
   - For every critical flow: step-by-step sequence across services
   - Actor → Service → Service → Database → Response

5. STATE MACHINES
   - For all stateful entities (e.g., job post, candidate, interview, round)
   - All states, transitions, triggers, and guards

6. QUEUE AND EVENT DEFINITIONS
   - Event name and schema
   - Producer service
   - Consumer service(s)
   - Retry and dead-letter policy

7. CACHING STRATEGY
   - What is cached per service
   - Cache key design
   - TTL and invalidation rules

8. ERROR HANDLING
   - Error taxonomy
   - Retry logic per failure type
   - Fallback behavior
   - User-facing error messaging

9. SECURITY RULES
   - Authorization checks per endpoint
   - Tenant isolation enforcement at data layer
   - Input sanitization rules

Format: Module by module. Precise enough that a developer can begin coding immediately.
```

**Input:** Phase 4 output  
**Output:** APIs, schemas, state machines, sequence flows

---

## Phase 6 — Presentation Data Dump

```
You are a product evangelist and strategic communicator.

Product: [PRODUCT NAME]
Full context: [PASTE PRD + ARCHITECTURE + HLD OUTPUTS]
Audience: [PRESENTATION AUDIENCE]
Slide count: [SLIDE COUNT]

Prepare a data dump for a [SLIDE COUNT]-slide presentation.
Give me content only — no formatting, no slide design instructions.

For each slide provide:
- Slide number and title
- 3–5 crisp data points or statements (numbers, benchmarks, facts)
- One "so what" conclusion line that makes the audience act

Cover in this order:
1.  Problem statement — pain in dollar terms
2.  Market size — TAM / SAM / SOM with growth rate
3.  Product overview — what it is in plain language
4.  How it works — end-to-end flow in 5 steps
5.  AI and automation advantage — what humans no longer need to do
6.  Competitive landscape — named competitors, gap table
7.  Product feature matrix — by user role
8.  Multi-tenant SaaS architecture — headline view
9.  Pricing and revenue model — tiers and unit economics
10. Cost savings for the customer — ROI with numbers
11. Infrastructure cost — per user tier, total at scale
12. Go-to-market strategy — channels, sequence, timeline
13. Revenue projections — Year 1 / 3 / 5
14. Roadmap — phased delivery with milestones
15. Team and execution plan
16. Risk and mitigation
17. Success metrics — KPIs with targets
18. Why now — market timing argument
19. Competitive moat — what makes this defensible
20. The ask — decision required, next steps

Source real market data. Every number must be credible.
Make every slide something a CFO or CTO would find convincing.
```

**Input:** Phase 2 + Phase 3 + Phase 4 outputs  
**Output:** 20-slide ready content

---

## Phase 7 — Screen by Screen Design Document

```
You are a senior UX architect and product designer.

Product: [PRODUCT NAME]
PRD input: [PASTE PHASE 2 OUTPUT]
User journeys: [PASTE PHASE 1 OUTPUT]
Design system: [PASTE THE FULL DESIGN SYSTEM BLOCK FROM THE TOP OF THIS DOCUMENT]

Prepare a screen-by-screen design specification for all interfaces:

SYSTEMS TO COVER:
- System 1: [e.g., Super Admin Panel — your company]
- System 2: [e.g., Client Admin Dashboard]
- System 3: [e.g., End User / Candidate Interface]

For every screen, provide:

SCREEN HEADER
- Screen name
- Which user role accesses this
- Purpose of this screen
- How the user arrives here (navigation path)

LAYOUT SPECIFICATION
- Layout pattern (sidebar + main / topnav + content / centered single column)
- Grid structure
- Responsive behavior at 1200px / 768px / 375px

SECTION-BY-SECTION BREAKDOWN
For every section on the screen:
- Section name and position
- Components present (list every component explicitly)
- Data displayed (field names and types)
- Actions available (buttons, links, interactions)
- Empty state design
- Loading state design
- Error state design

FORM SPECIFICATIONS (if applicable)
- Every field: label, input type, validation rules, error message
- Submit behavior and feedback

MODAL AND OVERLAY SPECS
- Trigger condition
- Content inside modal
- Confirm / cancel behavior
- Backdrop and focus behavior

NAVIGATION AND ROUTING
- Where each action routes to
- Back / breadcrumb behavior
- Deep link structure

NOTIFICATIONS AND FEEDBACK
- In-app notification triggers from this screen
- Toast / banner / inline feedback messages

Apply the design system strictly throughout.
Do not create visual designs.
Write specifications precise enough for a designer to build pixel-perfect in Figma.
Cover every screen, every state, every edge case.
```

**Input:** Phase 1 + Phase 2 outputs + Design System  
**Output:** Pixel-ready screen specs for Figma

---

## Phase 8 — Architecture Diagram Blueprint

```
You are a solutions architect preparing diagram-ready documentation.

Product: [PRODUCT NAME]
Architecture input: [PASTE PHASE 3 OUTPUT]

Prepare a structured blueprint for architecture diagrams.
Do not generate visuals. Produce structured text that a designer
can translate directly into Eraser, Lucidchart, Miro, or draw.io.

For each diagram:

DIAGRAM 1 — SYSTEM CONTEXT
- List every external actor
- List every external system
- Arrows: direction and label (what flows)
- System boundary box contents

DIAGRAM 2 — CONTAINER ARCHITECTURE
- Every deployable container / service
- Layer groupings (Frontend / Backend / AI / Data / Infra)
- Connections between containers with protocol label
- Cloud service boxes with service name

DIAGRAM 3 — DATA FLOW (per major workflow)
- Source → transformation steps → destination
- Sync vs async labels
- Queue and event labels

DIAGRAM 4 — AI AGENT ORCHESTRATION
- Input sources
- Agent decision tree
- Model calls
- Output destinations

DIAGRAM 5 — SECURITY AND TENANT ISOLATION
- Auth flow
- Tenant boundary enforcement points
- Encryption layers
- Audit trail path

DIAGRAM 6 — INFRASTRUCTURE AND SCALING
- Cloud region and availability zone layout
- Load balancer placement
- Auto-scaling groups
- CDN and edge layer
- Disaster recovery topology

For each component in every diagram:
- Component name
- Type (service / database / queue / model / gateway)
- Cloud service name if applicable
- Connects to (list)
- Data / event flowing on each connection

Format: Diagram by diagram, component by component.
Structured enough for direct import into any diagramming tool.
```

**Input:** Phase 3 output  
**Output:** Eraser / Lucidchart / Miro ready component lists

---

## Chaining Guide — Phase Execution Order

```
PHASE 1  →  Storyboard
             Input:  Raw idea
             Output: User journeys, personas, AI automation map
                ↓
PHASE 2  →  PRD
             Input:  Phase 1 output
             Output: Full product requirements, pricing, market data
                ↓
PHASE 3  →  Architecture Document
             Input:  Phase 2 output
             Output: Full cloud architecture, cost estimates
                ↓
PHASE 4  →  High Level Design (HLD)
             Input:  Phase 3 output
             Output: Module design, data flows, ADRs
                ↓
PHASE 5  →  Low Level Design (LLD)
             Input:  Phase 4 output
             Output: APIs, schemas, state machines, sequence flows
                ↓
PHASE 6  →  Presentation Data Dump
             Input:  Phase 2 + Phase 3 + Phase 4 outputs
             Output: 20-slide ready content
                ↓
PHASE 7  →  Screen by Screen Design Document
             Input:  Phase 1 + Phase 2 outputs + Design System
             Output: Pixel-ready screen specs for Figma
                ↓
PHASE 8  →  Architecture Diagram Blueprint
             Input:  Phase 3 output
             Output: Eraser / Lucidchart / Miro ready component lists
```

---

## Pro Rules for Maximum Output Quality

### Rule 1 — Chain Outputs
Never start a phase without the previous phase's output as input. The quality compounds with each phase.

### Rule 2 — Declare Constraints Upfront
Always state: cloud provider, team size, budget range, timeline, regulatory requirements, target markets. Constraints produce better output than open-ended prompts.

### Rule 3 — Force Alternatives
Add to every technical phase:
> *"Give me 3 alternative approaches with tradeoff comparison."*

### Rule 4 — Force Completeness
End every phase prompt with:
> *"Add anything missing that would make this world-class. Flag all open questions and risks."*

### Rule 5 — Separate Data from Format
Ask for data dumps first, formatting second. Never mix content generation with presentation formatting.

### Rule 6 — Lock the Design System
Paste the full design system block into every UI/UX phase. Never assume the model remembers it from a previous message.

### Rule 7 — Module by Module
For LLD and screen design, always process one module or one screen at a time for maximum depth and precision.

### Rule 8 — Validate Each Phase
Before moving to the next phase, ask:
> *"What is missing from this output that would cause downstream phases to be incomplete or incorrect?"*

---

## Quick Reference — Phase Summary Table

| Phase | Name | Input | Output | Tools |
|---|---|---|---|---|
| 1 | Storyboard | Raw idea | Journeys, personas, AI map | Claude / GPT |
| 2 | PRD | Phase 1 | Requirements, pricing, market | Claude / GPT |
| 3 | Architecture | Phase 2 | Cloud design, cost estimates | Claude / GPT |
| 4 | HLD | Phase 3 | Module design, ADRs | Claude / GPT |
| 5 | LLD | Phase 4 | APIs, schemas, state machines | Claude / GPT |
| 6 | Presentation | Phase 2+3+4 | 20-slide content | Claude / GPT |
| 7 | Design Doc | Phase 1+2+Design System | Figma-ready specs | Claude / GPT |
| 8 | Diagram Blueprint | Phase 3 | Diagram-ready components | Eraser / Lucidchart / Miro |

---

## Color Reference Card

| Token | Hex | Usage |
|---|---|---|
| Primary Blue | `#0A66C2` | Dominant brand color |
| Active Blue | `#004182` | Hover and active states |
| Background | `#F3F6F8` | Page background |
| Surface | `#FFFFFF` | Cards and panels |
| Border | `#E5E7EB` | All borders |
| Text Primary | `#111827` | Headings and body |
| Text Muted | `#6B7280` | Secondary text, placeholders |
| Success | `#057642` | Confirmations, passed states |
| Warning | `#B45309` | Caution messages |
| Error | `#B91C1C` | Error states, failures |

---

*Built for [PRODUCT NAME] — Adapt for any enterprise SaaS or AI product.*  
*Version 1.0 — Replace all `[VARIABLES]` before use.*
