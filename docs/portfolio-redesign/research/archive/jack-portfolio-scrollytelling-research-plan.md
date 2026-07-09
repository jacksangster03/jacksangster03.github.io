# Jack Sangster Portfolio Scrollytelling Redesign
## Research, Information Architecture, Visual Direction and Codex Build Plan

**Prepared:** 1 July 2026  
**Target repository:** `jacksangster03/jacksangster03.github.io`  
**Purpose:** Define a coherent redesign before implementation. This document separates narrative, content architecture, visual design, motion design, assets and engineering so an AI coding agent does not improvise the whole site in one pass.

---

# 1. Executive recommendation

Do not ask Codex or Claude Code to “make the portfolio cinematic” in one prompt.

The redesign should proceed through five controlled deliverables:

1. `PORTFOLIO-STRATEGY.md`  
   Defines the audience, positioning, content hierarchy and what the visitor should remember.

2. `DESIGN.md`  
   Defines typography, palette, layout, components, image treatment and visual constraints.

3. `MOTION.md`  
   Defines shared motion rules, ScrollTrigger behaviour, easing, pinning, responsive fallbacks, reduced motion and performance limits.

4. `STORYBOARD.md`  
   Defines the page-wide scroll narrative and transitions between domains.

5. `scenes/*.md`  
   Defines each complex visual independently, including its narrative purpose, scroll states, assets, implementation method and acceptance criteria.

Only after these files are reviewed should the agent build a prototype consisting of:

- the hero
- one domain chapter
- one flagship project chapter
- the mobile and reduced-motion fallbacks

The portfolio should not become four separate mini-websites. It should have one restrained core identity, with controlled domain-specific visual changes for biology, neuro, finance and software.

---

# 2. Current-site diagnosis

The current portfolio has strong evidence but presents it as a long CV.

## Current strengths

- Clear identity and readable typography
- Substantial project evidence
- Strong cross-disciplinary profile
- Direct links to projects and GitHub
- Simple static deployment
- Low technical risk and fast loading

## Current structural weaknesses

- All projects have nearly equal visual weight
- The About section explains the interdisciplinary story, but the page does not demonstrate it visually
- Skills are presented mainly as keyword inventories
- Experience appears before visitors see the strongest evidence
- Thirteen projects create fatigue
- There is little distinction between established expertise and emerging interests
- Existing animation is decorative rather than narrative
- A single large `index.html` makes complex scene development difficult

## Core redesign objective

The visitor should leave with one clear interpretation:

> Jack combines scientific literacy, quantitative judgement and technical execution to build decision systems across healthcare, finance and emerging neurotechnology.

The page should prove that statement through a sequence rather than repeat it in prose.

---

# 3. Audience and priority

## Primary audience

- Pharma technology and digital-health hiring managers
- Biotech data, AI and product teams
- Fintech and financial-intelligence teams
- Technical recruiters evaluating hybrid product-engineering candidates
- Collaborators, hackathon judges and research-oriented developers

## Secondary audience

- General software recruiters
- University and programme contacts
- Potential startup collaborators
- People discovering projects through GitHub

## Desired actions

The visitor should be able to:

1. Understand Jack’s positioning within 10 seconds
2. See the strongest projects within 30 seconds
3. Explore domain-specific work without reading every project
4. Verify technical depth through project detail
5. Reach GitHub, LinkedIn, email and CV easily
6. Use the site on mobile and with reduced motion

---

# 4. Content architecture

The site should be split into **narrative chapters**, not the existing résumé headings.

## Recommended top-level structure

```text
01  Opening
02  Operating system
03  Selected systems
04  Domain atlas
    04A Biology and computational science
    04B Neurotechnology and biosignals
    04C Markets and quantitative systems
    04D AI and software infrastructure
05  Experience and education
06  Project archive
07  Contact
```

## Why this structure works

- The opening establishes identity
- The operating-system chapter explains why the disciplines belong together
- Selected systems provides proof early
- The domain atlas lets visitors explore specialised work
- Experience and education support the proof instead of delaying it
- The archive retains breadth without making all projects cinematic

---

# 5. What belongs in each domain

Projects should be grouped by the problem domain they demonstrate, not only by technology.

## Biology and computational science

### Flagship work

- SMILES-IUPAC Translation
- Tox21 Toxicity Prediction
- Metabolix
- CHKB Q328R final-year research, presented as research background rather than a software project

### Supporting work

- DeepChem contribution
- Drug-discovery tools and molecular modelling
- Relevant components of SEIL
- Pharma Brief Automations where scientific sourcing matters

### Story

```text
Molecular structure
→ representation
→ data
→ prediction
→ scientific decision
```

### Visual language

- Warm scientific editorial foundation
- Molecular notation
- Annotation lines
- Specimen labels
- Restrained bioluminescent accents
- Real chemical strings and project outputs rather than fictional diagrams

---

## Neurotechnology and biosignals

This chapter should clearly distinguish current work from future direction.

### Current proof

- `eeg-motor-imagery-decoding`
- Neuroscience learning roadmap
- Cognix as a health-intelligence system
- TRIBE v2 exploration, if meaningful work can be described accurately

### Emerging direction

- EEG preprocessing
- Motor-imagery decoding
- MNE
- CSP and LDA
- Neural signal interpretation
- Digital biomarkers
- Adaptive human systems

### Story

```text
Biological structure
→ electrical activity
→ measured signal
→ filtering
→ feature extraction
→ interpretation
```

### Positioning label

Use:

```text
CURRENT FRONTIER
Neurotechnology, biosignals and adaptive health systems
```

Do not present neurotechnology as equivalent to years of established professional experience.

### Visual language

- Dark clinical observatory
- Thin signal traces
- Neural fields
- Clear channel labels
- One luminous accent
- Clinical precision rather than science-fiction neon

---

## Markets and quantitative systems

### Flagship work

- Briefly
- FIFA WC26 Model
- Queen’s Tower Capital models
- Stockhub analysis
- Pharma catalyst and market-intelligence automations where relevant

### Story

```text
Raw data
→ relevance filtering
→ model
→ uncertainty
→ decision
```

### Visual language

- Financial editorial layouts
- Dense but controlled numerical typography
- Grid lines
- Real charts
- Portfolio and event relationships
- No fake stock prices or decorative candlesticks

---

## AI and software infrastructure

### Flagship work

- Sentinel
- SEIL
- MatchKey
- OffScript
- Pharma Brief Automations

### Supporting work

- GeoMadrid
- Arcadia
- Elsewhere, when public
- Other products that demonstrate implementation breadth

### Story

```text
Inputs
→ model or agent
→ tools and data
→ governed workflow
→ user outcome
```

### Visual language

- System diagrams
- Interface windows
- Data routes
- Agent pathways
- Product screenshots
- Restrained terminal or blueprint motifs

---

# 6. Selected flagship projects

Only four or five projects should receive full scrollytelling chapters.

## Recommended five

### 1. SEIL

Why:
- Strong pharma-tech positioning
- Clear business result
- Healthcare AI governance
- Product, finance and technical architecture in one project

Custom interaction:
- A query enters
- It is classified by risk and intent
- It moves through one of seven routes
- Retrieval and review appear
- Interaction data returns as demand intelligence

### 2. Sentinel

Why:
- Immediate visual impact
- Strong award result
- Geospatial and real-time systems
- Existing 3D globe

Custom interaction:
- Globe begins quiet
- Conflict, seismic and flight layers appear
- A route is evaluated
- Hazard reporting and AI assistance join the scene

### 3. SMILES-IUPAC Translation

Why:
- Direct evidence of computational science
- Recognisable transformation
- DeepChem contribution
- Strong technical specificity

Custom interaction:
- A chemical structure or SMILES string enters
- Tokenisation is exposed
- Attention or sequence transformation appears
- IUPAC output resolves
- Bidirectionality is demonstrated

### 4. Briefly

Why:
- Strong finance and automation fit
- Active product
- Clear data-to-decision story
- Supports hiring targets in finance and intelligence

Custom interaction:
- Raw feeds enter
- Noise is filtered
- Holdings and catalysts are matched
- A morning brief assembles

### 5. EEG Motor Imagery or Cognix

Choose based on which has the stronger real implementation by build time.

If EEG:
- Show raw channels, preprocessing, CSP features and LDA classification

If Cognix:
- Show raw biometrics, deterministic scoring, readiness mode and future biosignal integration

## Projects remaining in archive

- MatchKey
- Tox21
- OffScript
- Arcadia
- GeoMadrid
- Metabolix
- FIFA WC26
- Pharma Brief Automations
- Other public projects

The archive should be filterable by:

```text
All
Science
Neuro
Finance
AI Systems
Products
```

---

# 7. Page-wide storyboard

## Chapter 1: Opening

### Purpose

Introduce identity quickly and signal that this is not a standard CV page.

### Copy direction

```text
JACK SANGSTER

I build systems where
science, markets and software meet.
```

Supporting line:

```text
Biochemistry at Imperial.
Management and computer science at IE.
Products across healthcare, finance and AI.
```

### Visual

A central abstract object changes between:

1. molecular structure
2. neural or data network
3. market signal
4. system graph

The object should remain abstract enough to connect the domains without becoming a literal collage.

### Interaction

- Full viewport
- Scroll maps to three or four controlled visual states
- Name and statement remain readable
- No long fake loader
- Direct links remain visible

---

## Chapter 2: Operating system

### Purpose

Explain why the profile is interdisciplinary rather than unfocused.

### Pinned narrative

```text
SCIENCE
Understand complex systems from first principles.

MARKETS
Quantify uncertainty, incentives and value.

SOFTWARE
Turn analysis into tools people can use.
```

Final state:

```text
Scientific literacy
+ quantitative judgement
+ technical execution
```

### Implementation

- Sticky or ScrollTrigger-pinned left rail
- Three text states
- Central visual changes meaningfully
- Simple vertical fallback on mobile

---

## Chapter 3: Selected systems

### Purpose

Show high-value proof early.

### Structure

- Five flagship project chapters
- Each chapter uses the same metadata framework
- Only the central scene changes

Shared metadata:

```text
Project number
Domain
Title
One-sentence problem
Role
Outcome
Technology
Link
```

---

## Chapter 4: Domain atlas

### Purpose

Allow visitors to explore the four domains without forcing a fixed long journey.

### Interaction options

Preferred:
- Four large chapters stacked vertically
- Each has a short signature animation
- Each links to relevant projects

Alternative:
- A domain index that expands one chapter at a time

Avoid:
- Four completely different navigation systems
- Hidden project content
- Horizontal-only navigation on mobile

---

## Chapter 5: Experience and education

### Purpose

Explain progression from Imperial to IE and from analysis to building.

### Suggested visual

```text
LONDON                         MADRID
2022                            2027
```

A timeline progresses through:

- Imperial biochemistry
- Equity research and consulting
- Finance Society leadership
- IE dual master’s
- Pharma, AI and neuro direction

### Content rule

Each role gets:

- date and location
- one-line responsibility
- one quantitative or meaningful result

A downloadable CV holds the full detail.

---

## Chapter 6: Project archive

### Purpose

Retain breadth.

### Structure

- Compact grid or editorial list
- Filters
- Search optional
- Project status label
- Real links
- No heavy custom animation

---

## Chapter 7: Contact

### Closing statement

```text
LET'S BUILD SOMETHING
THAT REQUIRES MORE THAN
ONE DISCIPLINE.
```

Include:

- email
- GitHub
- LinkedIn
- CV
- Madrid location
- Spain and UK work authorisation
- role interests

---

# 8. Visual design direction

## Recommended design lock

### Primary identity

**Scientific editorial**

Reference qualities:
- warm, credible and research-led
- large editorial typography
- annotation details
- material surfaces
- strong reading experience

### Technical structure

**Precision interface**

Reference qualities:
- clean grids
- restrained metadata
- exact component alignment
- useful diagrams
- no decorative SaaS clutter

### Cinematic motion

**Gallery pacing**

Reference qualities:
- full-screen chapter transitions
- large typographic moments
- deliberate reveals
- strong contrast changes
- limited simultaneous motion

### Neuro mode

**Clinical observatory**

Reference qualities:
- dark surfaces
- thin signal lines
- luminous but restrained accent
- precise labels
- real signal semantics

### Finance mode

**Financial broadside**

Reference qualities:
- oversized metrics
- editorial charts
- tabular data
- monochrome foundation
- minimal highlight colour

---

# 9. Design tokens

These are a starting point, not a final approved palette.

## Core colours

```css
--paper: #EEEAE2;
--paper-deep: #DDD7CC;
--ink: #111311;
--ink-soft: #5F625C;
--line: rgba(17, 19, 17, 0.16);

--night: #090C0C;
--night-soft: #111716;
--night-line: rgba(238, 234, 226, 0.14);

--signal: #B6FF43;
--signal-soft: rgba(182, 255, 67, 0.18);
```

## Domain accents

Prefer one shared signal colour. If domain distinction is needed, use very restrained secondary accents:

```css
--bio: #7CBF91;
--neuro: #B6FF43;
--finance: #E0B35A;
--systems: #82A7FF;
```

Do not display all four together frequently.

## Typography

Recommended pairing:

- Display serif or expressive editorial face for large statements
- Neutral grotesque for body and UI
- Monospace only for scientific strings, data and labels

Potential roles:

```text
Display:  clamp(4rem, 12vw, 11rem)
H2:       clamp(2.75rem, 7vw, 7rem)
H3:       clamp(1.75rem, 3vw, 3rem)
Body L:   1.25rem to 1.5rem
Body:     1rem to 1.125rem
Label:    0.7rem to 0.8rem
```

## Layout

- Twelve-column desktop grid
- Maximum readable width around 1440px
- Wide outer margins
- Long text limited to 60 to 72 characters per line
- Avoid endless cards
- Use section rules, labels and asymmetry
- Use rounded corners only where the product screenshot or interface requires them

---

# 10. Motion system

## Motion personality

The site should feel:

- deliberate
- intelligent
- calm
- precise
- cinematic at chapter boundaries
- responsive during interaction

It should not feel:

- bouncy
- game-like
- permanently in motion
- delayed
- over-smoothed
- dependent on cursor tricks

## Core motion vocabulary

Use only a few repeated behaviours:

1. Masked text reveal
2. Scrubbed scene transformation
3. Pinned explanatory sequence
4. Line drawing
5. Metric count or emphasis
6. Image or interface reveal
7. Chapter colour transition

## Timing

Non-scroll interactions:

```text
Micro interaction: 120–220ms
Small reveal:       300–500ms
Panel transition:   500–800ms
Chapter transition: 800–1200ms
```

Scroll-linked scenes should be controlled by scroll progress rather than fixed duration.

## Easing

Starting set:

```text
power2.out
power3.inOut
sine.inOut
```

Avoid applying elastic or back easing to serious scientific and finance interfaces.

## Pinning rules

- Maximum three consecutive pinned chapters
- A pinned chapter should explain a sequence, not merely hold a heading
- Avoid pinning on narrow mobile viewports
- Preserve browser history and anchor navigation
- Pin duration must be tied to content steps
- No nested scroll containers

## Reduced motion

When `prefers-reduced-motion: reduce` is active:

- Disable smooth scrolling
- Disable scrubbed transformations
- Show scene states as stacked static panels
- Preserve every piece of explanatory content
- Avoid autoplay ambient particles
- Keep navigation and project links identical

---

# 11. Scene specifications

## Scene 00: Hero convergence

### Narrative purpose

Show that science, markets and software form one operating model.

### Scroll states

```text
0–20%   Name and statement
20–40%  Molecular structure
40–60%  Network or signal structure
60–80%  Market or decision pattern
80–100% Unified systems object and entry into page
```

### Implementation preference

1. SVG or lightweight Canvas prototype
2. React Three Fiber only if the concept requires depth
3. No generated full-screen raster image as the functional scene

### Acceptance criteria

- Core statement readable at every state
- Interaction remains smooth on a mid-range phone
- Asset loads do not delay initial text
- Static fallback communicates the same idea

---

## Scene 01: Biology to computation

### Narrative purpose

Show how molecular and structural biology became computational work.

### Scroll states

```text
0–20%   Molecule or chemical representation
20–40%  Scientific annotation appears
40–60%  Representation becomes tokens or graph
60–80%  Model transformation
80–100% Predicted or translated output
```

### Real content options

- A valid SMILES example
- A corresponding IUPAC name
- Real tokenisation fragments
- A simplified Tox21 assay output
- A CHKB structural reference used accurately

### Implementation preference

- SVG
- CSS typography
- GSAP MorphSVG or controlled line/path animation
- Three.js only for an optional initial molecule

### Do not do

- Invent chemical outputs
- Use decorative DNA when the story is not genomics
- Use unreadable atom clouds
- Present a fake neural network diagram

---

## Scene 02: Neuro signal pipeline

### Narrative purpose

Show the path from electrical activity to interpretation.

### Scroll states

```text
0–15%   Quiet neural field or brain silhouette
15–30%  Signal propagation
30–45%  Multichannel raw EEG traces
45–60%  Filtering and artefact reduction
60–75%  Epoch or feature selection
75–90%  CSP or spatial feature representation
90–100% Classification or cognitive interpretation
```

### Real content options

- A short anonymised or public EEGMMIDB-derived waveform
- Channel labels
- Filter band
- CSP component visual
- LDA output
- Accuracy and validation details, only when real

### Implementation preference

- SVG for waveforms
- Canvas for larger channel counts
- Three.js or Canvas for initial field only
- GSAP ScrollTrigger for sequencing

### Mobile fallback

- Five stacked panels
- One compact waveform
- No pinned 3D field
- Text remains ahead of visuals

### Integrity rule

Label this section as current work or active frontier. Do not imply clinical diagnosis or mature BCI expertise.

---

## Scene 03: Finance decision pipeline

### Narrative purpose

Show how market noise becomes a portfolio-relevant decision.

### Scroll states

```text
0–20%   Headlines, releases and market data enter
20–40%  Irrelevant items fade
40–60%  Holdings and catalysts are linked
60–80%  Risk and signal hierarchy appears
80–100% Morning brief or alert resolves
```

### Real content options

- Sanitised Briefly output
- Public macro series
- Real portfolio-neutral example
- Event classification
- Confidence and source labels

### Implementation preference

- HTML and SVG
- Real chart library only if needed
- GSAP for reveal and relationship lines
- No generated financial UI

### Acceptance criteria

- Charts have readable axes and units
- Numbers are real or explicitly illustrative
- Animation clarifies filtering
- No ticker-wall cliché

---

## Scene 04: AI system architecture

### Narrative purpose

Connect domain knowledge to product implementation.

### Scroll states

```text
Input
→ classification
→ retrieval or model
→ tools and data
→ governance
→ output
→ feedback
```

### Best project

SEIL is the strongest candidate.

### Implementation preference

- SVG architecture graph
- HTML interface panels
- Animated route highlighting
- No 3D required

---

## Scene 05: Sentinel geospatial system

### Narrative purpose

Demonstrate spatial engineering and live-data integration.

### Scroll states

```text
Globe
→ conflict layer
→ flight layer
→ seismic layer
→ civilian route
→ hazard report
→ AI assistance
```

### Implementation preference

- Reuse a lightweight version or recording of the actual globe
- Lazy-load below the fold
- Use static map image on reduced-motion/mobile modes where needed

---

# 12. Image generation strategy

AI image generation is useful, but it should establish art direction rather than replace the interaction.

## Generate concept frames for

- hero atmosphere
- biology chapter atmosphere
- neuro chapter atmosphere
- finance chapter atmosphere

## Good image-generation targets

- abstract scientific environments
- microscopy-inspired fields
- editorial biological textures
- restrained laboratory atmospheres
- chapter poster art
- background depth layers

## Do not generate as final functional assets

- EEG data
- financial charts
- anatomy labels
- molecular outputs that need accuracy
- dashboards
- architecture diagrams
- text-heavy UI
- interactive states

## Recommended workflow

```text
1. Write scene specification
2. Generate one concept frame
3. Evaluate composition and mood
4. Convert useful qualities into tokens and layout rules
5. Rebuild the scene with HTML, SVG, Canvas or Three.js
6. Use the generated image only as supporting atmosphere when appropriate
```

The concept frame is a visual brief, not a screenshot to copy pixel-for-pixel.

---

# 13. Technical architecture

## Current-state implication

The existing single-file static page is appropriate for a basic portfolio, but it will become hard to maintain once it includes:

- multiple ScrollTrigger timelines
- project data
- responsive scene fallbacks
- asset preloading
- reduced-motion states
- reusable visual components
- testing

## Recommended migration

Use:

```text
Vite
React
TypeScript
GSAP
@gsap/react
ScrollTrigger
CSS Modules or well-structured global CSS
Optional React Three Fiber for one or two scenes
```

Why Vite rather than a full Next.js application:

- GitHub Pages is static
- The portfolio does not require server rendering
- Existing deployment remains simple
- Faster development and lower framework overhead
- Easy data-driven component structure

Next.js static export is also viable, but it adds limited value unless project case-study routing or image optimisation justifies it.

## Recommended source structure

```text
src/
├── app/
│   ├── App.tsx
│   └── routes.tsx
├── content/
│   ├── profile.ts
│   ├── projects.ts
│   ├── experience.ts
│   └── education.ts
├── components/
│   ├── layout/
│   ├── navigation/
│   ├── typography/
│   ├── projects/
│   └── motion/
├── scenes/
│   ├── HeroScene/
│   ├── OperatingSystemScene/
│   ├── BiologyScene/
│   ├── NeuroScene/
│   ├── FinanceScene/
│   ├── SeilScene/
│   └── SentinelScene/
├── hooks/
│   ├── useReducedMotion.ts
│   ├── useMediaQuery.ts
│   └── useScrollScene.ts
├── styles/
│   ├── tokens.css
│   ├── global.css
│   └── motion.css
└── assets/
    ├── images/
    ├── svg/
    ├── data/
    └── fonts/
```

## Content model

```ts
type Domain = "science" | "neuro" | "finance" | "systems";

type Project = {
  id: string;
  number: string;
  title: string;
  domain: Domain[];
  status: "live" | "complete" | "in-progress" | "research";
  prominence: "flagship" | "archive";
  statement: string;
  problem: string;
  contribution: string[];
  outcomes: {
    label: string;
    value: string;
  }[];
  technologies: string[];
  links: {
    label: string;
    href: string;
  }[];
};
```

---

# 14. Agent and skill setup

## Refero MCP

Use for:

- visual references
- typography
- palette
- component systems
- editorial layouts
- visual motifs

Do not expect Refero alone to define the complete scroll choreography.

## Official GSAP skills

The official `greensock/gsap-skills` repository provides agent guidance for:

- GSAP core
- timelines
- ScrollTrigger
- plugins
- React
- performance
- lifecycle and cleanup

Recommended installation:

```bash
npx skills add https://github.com/greensock/gsap-skills
```

or through the Claude Code plugin marketplace where supported.

## Reference sources

Use:

- Refero for visual systems
- GSAP official demos and skills for implementation
- Codrops for advanced scene patterns
- Real scientific and financial data for content
- Existing project screenshots and code as primary proof

## Rule for agent research

Every selected reference must record:

```text
Source
What is being borrowed
Why it fits
What must not be copied
Implementation method
Licence or usage constraint
Mobile fallback
Performance risk
```

---

# 15. Documentation package to create in the repository

```text
docs/portfolio-redesign/
├── README.md
├── PORTFOLIO-STRATEGY.md
├── RESEARCH-LEDGER.md
├── DESIGN.md
├── MOTION.md
├── STORYBOARD.md
├── CONTENT-MAP.md
├── ASSET-DIRECTION.md
├── PERFORMANCE.md
├── ACCESSIBILITY.md
└── scenes/
    ├── 00-hero.md
    ├── 01-operating-system.md
    ├── 02-biology.md
    ├── 03-neuro.md
    ├── 04-finance.md
    ├── 05-seil.md
    ├── 06-sentinel.md
    ├── 07-experience.md
    └── 08-contact.md
```

## Purpose of each file

### `README.md`

Project status and order of operations.

### `PORTFOLIO-STRATEGY.md`

Audience, positioning, priorities and success criteria.

### `RESEARCH-LEDGER.md`

All references and why they were selected or rejected.

### `DESIGN.md`

Shared visual system.

### `MOTION.md`

Shared motion grammar and engineering constraints.

### `STORYBOARD.md`

Page-level narrative and transitions.

### `CONTENT-MAP.md`

Current content, new location, edits needed and removals.

### `ASSET-DIRECTION.md`

Image, video, SVG, data and screenshot requirements.

### `PERFORMANCE.md`

Budgets and testing.

### `ACCESSIBILITY.md`

Reduced motion, keyboard, contrast, semantics and touch.

### `scenes/*.md`

Self-contained implementation briefs.

---

# 16. Performance budget

## Targets

```text
Largest Contentful Paint: under 2.5s on a representative mobile connection
Cumulative Layout Shift: under 0.1
Interaction to Next Paint: under 200ms where practical
Initial JavaScript: target under 250KB compressed
Initial hero media: target under 1.5MB
Active WebGL canvases: maximum 1
```

## Rules

- Lazy-load all heavy scenes below the hero
- Dispose Three.js resources on unmount
- Pause ambient animation when off-screen
- Prefer transforms and opacity
- Avoid permanent blur filters
- Avoid scroll listeners that force layout
- Use `gsap.context()` or `useGSAP()` cleanup
- Test Safari iOS early
- Do not add Lenis until native scrolling works correctly
- Smooth scrolling must not be required for the experience

---

# 17. Accessibility requirements

- Semantic section structure
- Meaningful heading order
- Keyboard-accessible navigation
- Visible focus styles
- Text remains selectable
- No content available only on hover
- Every project link has a clear label
- Charts include textual summaries
- Decorative Canvas and WebGL use `aria-hidden`
- Reduced-motion mode preserves narrative
- Colour is not the sole domain indicator
- Mobile tap targets at least 44px
- Background transitions preserve contrast

---

# 18. Build sequence

## Phase 0: Preserve current site

- Create a redesign branch
- Record Lighthouse baseline
- Capture desktop and mobile screenshots
- Preserve the existing deployed version until replacement is validated

## Phase 1: Research and reference lock

Deliver:

- research ledger
- three possible visual directions
- one selected direction
- no code changes

## Phase 2: Content architecture

Deliver:

- project categorisation
- flagship selection
- edited copy
- content map
- no complex animation

## Phase 3: Documentation

Deliver:

- `DESIGN.md`
- `MOTION.md`
- `STORYBOARD.md`
- scene files
- performance and accessibility specifications

## Phase 4: Static skeleton

Build:

- application structure
- navigation
- chapter layout
- content data
- archive
- responsive typography
- no heavy animations

## Phase 5: Vertical prototype

Build:

- hero
- operating-system sequence
- neuro scene
- one flagship case study
- mobile fallback
- reduced-motion fallback

Review before continuing.

## Phase 6: Remaining scenes

Build one scene at a time with acceptance checks.

## Phase 7: Optimisation

- asset compression
- device testing
- Lighthouse
- motion tuning
- keyboard and reduced-motion testing

## Phase 8: Deployment

- deploy preview
- compare against old page
- confirm links and metadata
- merge only after visual review

---

# 19. Codex research prompt

Use the following prompt before allowing Codex to modify the site.

```text
You are preparing a research and architecture package for the redesign of
jacksangster03.github.io.

Do not modify application code.

Read:
- the current repository
- its existing content and links
- any project-specific CLAUDE.md or AGENTS.md
- docs/portfolio-redesign/ if it exists

Objective:
Design a coherent scrollytelling portfolio for Jack Sangster. The portfolio must
present one integrated profile across computational biology, neurotechnology,
quantitative finance and AI/software systems.

Research tasks:

1. Audit the current site:
   - content hierarchy
   - current architecture
   - accessibility
   - performance
   - maintainability
   - strongest and weakest content

2. Audit the available projects and classify each into:
   - biology and computational science
   - neurotechnology and biosignals
   - finance and quantitative systems
   - AI and software infrastructure
   Some projects may have multiple domains.

3. Recommend:
   - four or five flagship projects
   - archive projects
   - copy that should be shortened
   - claims that require verification
   - distinctions between established work and emerging interests

4. Use Refero MCP to research:
   - scientific editorial systems
   - clinical observatory interfaces
   - financial editorial and intelligence systems
   - precise technical interfaces
   - cinematic portfolio pacing

5. Use primary or official sources to research:
   - GSAP ScrollTrigger implementation
   - official GSAP agent skills
   - accessible reduced-motion patterns
   - React and GSAP lifecycle
   - performance for Canvas, SVG and WebGL

6. For every visual or motion reference, record:
   - source
   - what is useful
   - what must not be copied
   - relevant scene
   - implementation method
   - mobile fallback
   - performance risk
   - licence where relevant

7. Produce proposals for:
   - DESIGN.md
   - MOTION.md
   - STORYBOARD.md
   - CONTENT-MAP.md
   - ASSET-DIRECTION.md
   - PERFORMANCE.md
   - ACCESSIBILITY.md
   - one scene file for every major chapter

Constraints:
- Do not implement the redesign.
- Do not install packages.
- Do not generate images.
- Do not modify persistent project files.
- Return findings and proposed file contents for review.
- Prefer a restrained coherent system over many unrelated effects.
- Treat real project outputs and real data as primary visual material.
- Do not overstate Jack's neurotechnology experience.
```

---

# 20. Codex implementation prompt after approval

```text
Implement only Phase 4 and the Phase 5 vertical prototype described in
docs/portfolio-redesign/.

Read every approved document before making changes.

Scope:
- migrate the current content into the approved component and data structure
- implement the static page skeleton
- implement the hero
- implement the operating-system sequence
- implement the neuro scene
- implement one approved flagship project scene
- implement mobile and reduced-motion variants
- preserve all valid external links
- preserve SEO metadata
- keep the existing site deployable until the new build passes validation

Do not:
- implement the remaining custom scenes
- invent project metrics
- invent scientific or financial data
- add an unapproved visual library
- introduce smooth scrolling until the native-scroll version passes
- use generated images as data visualisations
- modify content outside the approved content map

Required validation:
- production build
- no console errors
- keyboard navigation
- prefers-reduced-motion
- iPhone-width layout
- desktop layout
- Lighthouse report
- no broken links
- no overflow
- GSAP cleanup on unmount
- no more than one active WebGL canvas

At the end, report:
- files changed
- architectural decisions
- deviations from the approved documents
- validation results
- remaining work
```

---

# 21. Decisions to make before implementation

1. **Flagship neuro project**  
   EEG motor-imagery pipeline or Cognix?

2. **Framework**  
   Vite React TypeScript is recommended. Confirm before migration.

3. **Primary visual reference**  
   Select one Refero system as the dominant reference.

4. **Hero method**  
   SVG/Canvas first or React Three Fiber from the start?

5. **Project detail pages**  
   Single long page only or separate case-study routes?

6. **CV**  
   Add downloadable PDF or link elsewhere?

7. **Photography**  
   Use a portrait, project-only imagery or no personal photography?

8. **Generated art**  
   Approve concept frames before any are used in production.

---

# 22. Final recommendation

The best final structure is:

```text
Hero
→ interdisciplinary operating system
→ flagship proof
→ biology
→ neuro
→ finance
→ AI systems
→ experience and education
→ complete project archive
→ contact
```

However, the flagship proof and domain chapters should be interwoven so the page does not repeat projects twice in full. A project can be introduced in its domain and listed compactly in the archive.

The design system should remain one coherent scientific-editorial identity. Biology, neuro, finance and software should alter the data, imagery and scene behaviour, not replace the typography, grid and navigation every time.

The highest-value next action is to commit this research package to a redesign branch, run the research-only Codex prompt and review the resulting reference lock before any implementation.
