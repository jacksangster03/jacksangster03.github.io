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

## 12A. AI asset production system: Higgsfield, motion, sound and FFmpeg

### 12A.1 Final tool recommendation

Use Higgsfield as an **asset studio**, not as the runtime of the website.

Recommended stack:

| Task | Primary tool | Why | Production rule |
|---|---|---|---|
| Master still frames and visual continuity | Nano Banana Pro | Strong prompt adherence, spatial control and high-resolution image output | Build one approved keyframe per chapter before attempting motion |
| Fast prompt and composition tests | Nano Banana 2 Lite | Lower-cost iteration | Use only for rough exploration, not final chapter art |
| Controlled image-to-video loops | Kling 3.0 | Reference consistency, exact-duration clips and multi-shot support | Animate one restrained action per clip |
| Multi-shot transitions and clips that genuinely need integrated sound | Seedance 2.0 | Multimodal inputs, multi-camera sequences and native audio | Reserve for chapter trailers or project demos, not every background |
| Separate ambience or designed sound moments | Seed Audio 1.0 or a licensed sound library | Can produce speech and ambience independently | Sound must be optional and user initiated |
| Editing, trimming, looping, compression and web delivery | FFmpeg | Deterministic local processing and repeatable output | Every generated clip passes through a reproducible export script |
| Scroll choreography and factual visuals | GSAP, SVG, Canvas and HTML | Precise, accessible and tied to real data | Generated media never replaces EEG traces, charts, labels or architecture diagrams |

**Do not generate the whole portfolio as one continuous AI video.** Long generated sequences drift in geometry, visual identity and factual detail. Instead, create six to eight short visual loops that share one art direction. The page scroll controls opacity, crop, depth and transitions between them.

### 12A.2 Model selection rules

Use **Nano Banana Pro** when the outcome is a still image, a texture, a chapter poster or the first frame of a video. Higgsfield's own prompting guide recommends specifying subject, composition, action, style, lighting and constraints. It also recommends explicit negative constraints for factual and geometric consistency.

Use **Kling 3.0** for 4-8 second image-to-video loops where the first frame must remain recognisable. Prefer one camera move and one environmental motion. Do not ask for a molecule, waveform, chart and interface to transform simultaneously.

Use **Seedance 2.0** when a sequence needs multiple connected shots, several reference assets or synchronized sound. It supports image, video and audio references and can generate clips up to 15 seconds. For this portfolio, use it selectively for a 10-15 second showreel, a Sentinel transition or a standalone social teaser.

Use **Seed Audio 1.0** only for optional sonic branding, a social trailer or a user-triggered case-study film. Do not autoplay audio when the portfolio opens. A recruiter should be able to browse the entire page silently.

### 12A.3 Shared art-direction lock

Every generated chapter frame must follow this shared visual constitution:

```text
FORMAT
Cinematic scientific-editorial still, photorealistic material rendering,
controlled studio realism, premium museum-installation quality, 16:9 landscape,
composition safe for a responsive website crop, central subject inside the middle 60%,
clean negative space for typography, no embedded text.

MATERIAL LANGUAGE
Warm off-white paper, smoked glass, dark graphite metal, translucent resin,
fine etched lines, restrained luminous lime signal, subtle amber and blue secondary light.

CAMERA
Full-frame cinema camera, 50 mm or 65 mm lens unless otherwise specified,
physically plausible depth of field, controlled perspective, no extreme fisheye.

LIGHTING
Soft directional key light, low-intensity volumetric atmosphere,
credible reflections, deep blacks without crushed detail, no neon nightclub look.

MOOD
Intelligent, calm, exact, research-led, cinematic but not fantastical.

GLOBAL NEGATIVE CONSTRAINTS
No words, letters, logos, watermarks, fake interface text, random numbers,
extra screens, stock-photo people, cyberpunk city, excessive neon, oversaturated colours,
cheap holograms, tangled anatomy, incorrect molecular diagrams, decorative DNA,
fake stock charts, illegible labels, warped geometry, duplicated objects,
heavy bloom, lens dirt, chromatic aberration or visual clutter.
```

Create a single **reference board** first: one hero frame, one material macro and one palette strip. Reuse those outputs as image references for every later generation. Do not rely on text prompts alone to preserve continuity.

### 12A.4 Asset inventory and naming

```text
public/media/
├── hero/
│   ├── hero-master.png
│   ├── hero-loop.webm
│   ├── hero-loop.mp4
│   └── hero-poster.avif
├── biology/
├── neuro/
├── finance/
├── systems/
├── sentinel/
├── experience/
└── audio/
```

Naming convention:

```text
<section>-<shot>-v<iteration>-<ratio>.<ext>
hero-convergence-v03-16x9.png
neuro-signal-field-v02-16x9.webm
sentinel-orbit-v04-16x9.mp4
```

Retain the prompt, model, generation settings, source images and generation date beside each approved asset in `docs/portfolio-redesign/ASSET-LEDGER.md`.

### 12A.5 Prompt 01: hero convergence object

**Purpose:** Establish one visual object that plausibly connects molecular science, neural signals, market information and software systems without becoming a literal collage.

**Nano Banana Pro still prompt:**

```text
Create a cinematic scientific-editorial hero image for a premium interdisciplinary portfolio.

SUBJECT
One central suspended object built from a precise translucent resin core surrounded by a sparse
three-dimensional lattice. The lattice subtly combines four visual behaviours without literal icons:
small molecular-scale nodes and bonds, hair-thin signal filaments, ordered market-like trajectories
and clean system-routing paths. The object must read as one engineered artefact, not four objects
pasted together.

COMPOSITION
16:9 landscape. Object centred slightly right of frame, occupying approximately 42% of the width.
Leave generous dark negative space on the left and upper-left for large white editorial typography.
Camera at eye level, 65 mm lens, three-quarter view, controlled shallow depth of field. Preserve a
clean silhouette at mobile crops.

MATERIALS
Smoked glass, translucent resin, dark graphite micro-structure, tiny etched metallic connectors.
One restrained lime-green signal moves through selected paths. No rainbow colours.

ENVIRONMENT
Minimal black scientific gallery with a warm off-white floor plane fading into darkness. Almost
imperceptible atmospheric particles, like dust in a museum beam, not outer space.

LIGHTING
Soft warm key from upper left, cold narrow rim from rear right, physically accurate internal
refraction, subtle caustics, deep but readable shadows.

QUALITY
Photorealistic product cinematography, museum installation, extremely clean geometry, premium
material realism, 4K detail, no text.

NEGATIVE CONSTRAINTS
No brain, no DNA helix, no candlestick chart, no laptop, no robot, no obvious circuit board,
no sci-fi spaceship, no floating UI, no labels, no logos, no excessive glow, no tangled wires,
no duplicated nodes, no asymmetrical deformation.
```

**Kling 3.0 image-to-video motion prompt:**

```text
Use the supplied hero image as the exact first-frame and identity reference. Create a seamless
6-second cinematic loop. The camera performs an almost imperceptible 4% clockwise orbit and a 2%
slow push-in. Inside the object, one restrained lime signal travels through three connected routes,
briefly illuminating nearby nodes before fading. The resin core breathes with a very subtle internal
light pulse. Dust particles drift slowly. Keep the object's geometry, materials, scale and silhouette
locked. End in a pose that can crossfade invisibly back to the opening frame.

No new objects, no morphing, no camera shake, no fast rotation, no text, no strong bloom, no colour
shift and no changes to the background composition.
```

**Website motion treatment:** Use the generated clip only as a muted atmospheric layer. Scroll progress should reveal SVG overlays that mark `SCIENCE`, `MARKETS` and `SOFTWARE`. Do not try to bake those labels into the video.

### 12A.6 Prompt 02: biology to computation

**Purpose:** Create a realistic material bridge from molecular structure to computational representation.

**Nano Banana Pro still prompt:**

```text
Create a photorealistic scientific-editorial chapter image about molecular representation becoming
computation.

SUBJECT
A single precise ball-and-stick molecular model suspended above a warm laboratory work surface.
The physical model transitions only in material treatment toward the right: left side appears as
machined graphite and translucent resin atoms, while the right side resolves into a sparse ordered
field of small luminous nodes and etched graph connections. The transition must feel like an
analytical representation of the same structure, not magical disintegration.

COMPOSITION
16:9. Molecule spans the middle third horizontally. Leave the leftmost 28% and lower-left area quiet
for chapter copy. 50 mm macro-influenced lens, slightly elevated three-quarter angle. Fine depth of
field but keep the complete molecular silhouette recognisable.

ENVIRONMENT
Warm off-white scientific paper, a smoked glass specimen plate and one precise metal annotation
pin. Background is a dark-to-warm gradient, editorial rather than clinical.

LIGHTING
Soft warm laboratory key, faint green internal signal on the computational side, controlled shadow
on the paper surface.

STYLE
Premium scientific journal cover photographed as a real installation. Exact geometry, restrained
palette, highly realistic materials, no text.

NEGATIVE CONSTRAINTS
No DNA helix, no cells, no test tubes, no medical cross, no fictional atom labels, no equations,
no floating dashboard, no rainbow bonds, no explosive particle effect, no extra molecules,
no incorrect embedded chemical notation.
```

**Kling 3.0 motion prompt:**

```text
Create a 7-second seamless image-to-video loop from the supplied still. Camera remains nearly fixed
with a slow 3% lateral move from left to right. A thin scanning light passes across the molecule.
As the scan reaches each bond, a corresponding graph node on the right becomes softly visible.
The physical molecule itself does not deform or change atom count. Fine paper fibres and a faint
volumetric beam move naturally. End with the same overall light balance as the first frame.

No atom movement, no bond rearrangement, no text, no new molecular fragments, no dramatic zoom,
no magical dissolve and no inaccurate chemistry.
```

**Accuracy layer:** Overlay the real SMILES string, tokenisation and IUPAC output using HTML/SVG. The generated image provides material atmosphere only.

### 12A.7 Prompt 03: neuro signal observatory

**Purpose:** Convey biosignal measurement and interpretation without implying clinical diagnosis or futuristic mind reading.

**Nano Banana Pro still prompt:**

```text
Create a dark clinical-observatory image for a portfolio chapter on EEG motor-imagery decoding.

SUBJECT
A translucent anatomically plausible human head form in side profile, made from smoked optical
resin, mounted like a precision research instrument. A sparse array of small matte electrode points
sits on the scalp surface in a plausible EEG-like distribution. One subtle wave of electrical activity
travels across the sensor field. Behind the head, several ultra-thin horizontal signal traces exist as
abstract light reflections, not readable data.

COMPOSITION
16:9. Head occupies the right 42% of frame, facing left. Leave wide negative space at left for title
and explanatory steps. 85 mm portrait lens, profile view, camera level with temporal region. Strong,
clean silhouette and generous breathing room.

ENVIRONMENT
Near-black clinical room, graphite instrument base, barely visible calibration grid in the far
background. No hospital patient, no headset product advertisement.

LIGHTING
Narrow cool rim around the head, very restrained lime signal at selected sensors, soft neutral fill
that preserves resin detail. Deep blacks, no nightclub neon.

STYLE
Photorealistic scientific instrument photography, clinically precise, calm, premium, credible,
subtle atmosphere, 4K, no text.

NEGATIVE CONSTRAINTS
No exposed brain, no glowing cybernetic eyes, no helmet, no cables entering skin, no medical claims,
no diagnostic interface, no fake channel labels, no psychedelic colours, no lightning bolts,
no distorted anatomy, no extra facial features and no aggressive sci-fi styling.
```

**Kling 3.0 motion prompt:**

```text
Animate the supplied neuro observatory frame into a restrained 6-second loop. Keep the head,
electrodes and camera locked. A single low-amplitude signal pulse travels from posterior to anterior
across a few electrode points. Background reflections respond with a faint delayed waveform.
The camera performs a 2% slow push-in. Resin reflections shift physically with the camera.
Return the light pulse to zero before the final frame for a clean loop.

No facial movement, no head rotation, no new electrodes, no electric sparks, no data labels,
no dramatic pulsing and no colour changes.
```

**Accuracy layer:** Draw actual EEGMMIDB traces, channel names, filter band and CSP/LDA outputs in SVG or Canvas above the atmospheric frame.

### 12A.8 Prompt 04: finance signal filtering

**Purpose:** Represent information filtering and decision relevance without fake prices or ticker-wall clichés.

**Nano Banana Pro still prompt:**

```text
Create a cinematic financial-editorial still about turning noisy information into a clear decision.

SUBJECT
A physical tabletop installation made from hundreds of thin translucent paper slips and narrow glass
strips entering from the upper-left in a loose, chaotic stream. As they cross a precise matte-black
filtering gate at centre, only a small number emerge on the right as aligned, evenly spaced amber and
white information cards. One lime indicator marks a single high-relevance item. All surfaces are
blank and contain no text or numbers.

COMPOSITION
16:9, top-down oblique view at approximately 35 degrees. Flow travels diagonally left to right.
Leave the upper-right and lower-right areas sufficiently quiet for metrics and copy. 50 mm lens,
controlled perspective, no fisheye.

MATERIALS
Warm paper, clear glass, graphite metal, subtle amber edge light, one restrained lime signal.

ENVIRONMENT
Premium financial newspaper art direction translated into a real studio installation. Warm off-white
surface with fine grid embossing. Dark background falloff.

LIGHTING
Crisp editorial side light, precise shadows, high micro-contrast, no glossy casino aesthetic.

NEGATIVE CONSTRAINTS
No stock tickers, no candlestick charts, no currency symbols, no Wall Street skyline, no traders,
no laptops, no fake UI, no embedded words, no random numbers, no red-green market cliché,
no flying money and no excessive data particles.
```

**Kling 3.0 motion prompt:**

```text
Create a seamless 7-second loop. Incoming blank paper and glass strips move slowly toward the central
filter. Most dim and pass beneath the surface while four selected strips continue to the right and
align precisely. A single restrained lime indicator activates on one selected strip. Camera remains
stable with a very slow 3% forward dolly. All blank surfaces stay blank. Finish with the composition
matching the opening state through a soft cyclical flow.

No text generation, no price charts, no sudden acceleration, no object duplication, no paper storm,
no camera shake and no dramatic glow.
```

**Accuracy layer:** Real Briefly headlines, confidence labels, holdings matches and charts remain HTML/SVG components controlled by scroll.

### 12A.9 Prompt 05: SEIL governed AI pathway

**Purpose:** Visualise a governed healthcare-AI workflow as a physical routing system.

**Nano Banana Pro still prompt:**

```text
Create a premium scientific systems image representing a governed medical-information workflow.

SUBJECT
A physical routing instrument on a dark graphite table. One translucent input capsule enters from
the left and reaches a circular classification junction. Seven fine etched pathways branch from the
junction toward distinct destinations. Three routes pass through smoked-glass review chambers,
one route reaches a warm paper evidence archive and one route returns through a feedback ring.
The system is sparse, clean and mechanically plausible. No route contains text.

COMPOSITION
16:9, isometric three-quarter view from above, 55 mm lens. Main junction placed slightly left of
centre. Reserve the rightmost 30% for explanatory copy and real interface panels. Keep paths legible
and avoid overlap.

MATERIALS
Dark graphite, smoked glass, translucent resin, warm paper archive, one lime active route and subtle
blue governance lighting.

LIGHTING
Museum-grade product lighting with controlled reflections. Active route glows softly but does not
illuminate the entire scene.

STYLE
Photorealistic systems architecture built as a precision physical model, credible healthcare and
research tone, no futuristic hospital clichés, no text.

NEGATIVE CONSTRAINTS
No chatbot face, no robot doctor, no medical cross, no patient, no floating dashboard, no labels,
no random icons, no tangled circuit board, no excessive routes, no bright cyan holograms,
no impossible geometry and no generic server-room imagery.
```

**Kling 3.0 motion prompt:**

```text
Animate a controlled 8-second route demonstration. The translucent input capsule enters slowly,
pauses at the classification junction and activates one lime route. The signal moves through a
smoked-glass review chamber, reaches the evidence archive and returns through the feedback ring.
Other routes remain dormant and structurally unchanged. Camera makes a restrained 4% isometric
arc. End with the capsule outside frame and all lights returned to baseline so the loop can restart.

No new routes, no route crossing, no text, no fast pulses, no dramatic machinery and no camera spin.
```

**Accuracy layer:** The seven routes, risk labels, content metadata and review states must be recreated from the real SEIL design in SVG/HTML.

### 12A.10 Prompt 06: Sentinel geospatial intelligence

**Purpose:** Produce a realistic cinematic backdrop for Sentinel while preserving the actual globe and data layers as code or captured project output.

**Nano Banana Pro still prompt:**

```text
Create a cinematic geospatial-intelligence chapter frame for a civilian safety and route-awareness
system.

SUBJECT
A large dark glass globe suspended above a graphite instrument base in a minimal operations gallery.
The visible geography is recognisable as the Mediterranean, Europe, North Africa and the Middle East,
but coastlines should be subtle and not presented as a political map. A small number of fine arc
routes cross the surface. Three restrained layer behaviours are suggested through material only:
a faint amber seismic ripple, a thin white flight arc and a muted red conflict-region haze. No labels,
flags or borders.

COMPOSITION
16:9. Globe centred slightly left, occupying 48% of frame. Leave right side clear for project copy and
actual interface overlays. Camera at a low three-quarter orbital angle, 50 mm lens. Maintain a strong
circle silhouette.

ENVIRONMENT
Black museum-scale operations room, subtle floor reflection, no people, no wall of screens.

LIGHTING
Cool rim light around the globe, soft warm reflection from below, very restrained atmospheric haze,
high material realism.

NEGATIVE CONSTRAINTS
No military command centre, no weapons, no missiles, no national flags, no labels, no random city
names, no glowing cyberpunk continents, no inaccurate extra land masses, no satellite clutter,
no excessive flight paths and no apocalyptic imagery.
```

**Kling 3.0 motion prompt:**

```text
Create an 8-second seamless orbit loop from the reference frame. The camera makes a slow 6-degree
clockwise orbit while the globe rotates approximately 4 degrees in the opposite direction. One white
flight arc draws on, one amber seismic ripple expands and fades and one muted hazard haze breathes
very slightly. Geography, coastlines and globe proportions remain locked. Return all transient layers
to baseline before the final frame.

No new continents, no labels, no explosions, no rapid rotation, no camera shake, no dramatic zoom,
no added satellites and no changes in colour palette.
```

**Preferred production method:** Use a recording or reduced version of the real Sentinel globe whenever possible. The generated globe is a poster and fallback, not evidence of the actual implementation.

### 12A.11 Prompt 07: experience transition, London to Madrid

**Purpose:** Provide a human, geographic breath between technical chapters without using a generic portrait.

**Nano Banana Pro still prompt:**

```text
Create a refined editorial still representing an academic and professional transition from London
to Madrid.

SUBJECT
A long physical timeline built across a warm architectural table. At the far left, a small abstract
stone-and-brass form evokes London academic architecture without reproducing a landmark. At the far
right, a warmer terracotta-and-glass form evokes Madrid contemporary architecture. Between them,
five precise milestones are represented by small material changes: laboratory glass, financial paper,
a dark software module, a blue governance tile and a lime signal element. No words or dates.

COMPOSITION
Ultra-wide 16:9 landscape, timeline crossing lower middle of frame. Large negative space above for
timeline copy. Camera at table height with a 65 mm lens and deep-enough focus to preserve both ends.

LIGHTING
Cool daylight from the left gradually transitioning to warm golden light on the right, physically
continuous and subtle.

STYLE
Premium architecture-magazine still life, scientific editorial materials, calm and credible.

NEGATIVE CONSTRAINTS
No Big Ben, no Spanish flag, no aeroplane, no suitcase, no graduation cap, no portrait, no skyline
collage, no text, no logos and no tourist-postcard styling.
```

**Motion prompt:**

```text
Animate a 7-second slow lateral camera move from the cooler left side toward the warmer right side.
Small milestone materials catch light one after another. No objects move position. The lime signal
activates only at the final milestone, then returns to baseline. Preserve the timeline geometry and
allow a gentle crossfade loop.
```

### 12A.12 Prompt 08: closing contact field

**Purpose:** End with visual resolution rather than another complex demo.

**Nano Banana Pro still prompt:**

```text
Create a minimal cinematic closing frame for an interdisciplinary portfolio.

SUBJECT
The same central resin-and-graphite object from the hero, now resting open and resolved on a warm
off-white surface. Its internal pathways converge into one clear lime line that exits toward the lower
right edge, suggesting continuation beyond the frame. The object is quieter, simpler and more human
than in the opening image.

COMPOSITION
16:9. Object positioned in lower-left third, large clean negative space across the upper and right
areas for the closing statement and contact links. 65 mm lens, slightly elevated camera, crisp but
soft editorial depth of field.

LIGHTING
Warm dawn-like key light, faint cool rim retained from the hero, gentle long shadow, no dramatic haze.

NEGATIVE CONSTRAINTS
No hands, no people, no envelope icon, no social-media logos, no text, no excessive glow,
no new object design and no visual clutter.
```

**Motion prompt:**

```text
Create a subtle 5-second loop. Camera remains effectively static. Internal light converges slowly
into the single outgoing line, then dims back to its initial state. One soft shadow shift suggests
changing daylight. Preserve all geometry and leave the negative space completely empty.
```

### 12A.13 Continuity workflow

For each chapter:

1. Generate 12-20 low-cost composition candidates with Nano Banana 2 Lite.
2. Select two compositions only.
3. Rebuild the preferred composition with Nano Banana Pro using the global art-direction lock.
4. Use the approved hero/material references with every chapter generation.
5. Produce one master 4K still.
6. Create two motion variants in Kling 3.0: a conservative loop and a slightly more cinematic loop.
7. Keep the conservative version unless the cinematic version clearly improves comprehension.
8. Export a still poster even when video is approved.
9. Record model, prompt, reference files, generation date and approval status in the asset ledger.
10. Test the crop at 1440x900, 390x844 and 768x1024 before approving an asset.

### 12A.14 Motion improvement rules

The main failure mode in AI video is asking too much of one shot. Improve stability through these rules:

- Begin from an approved image instead of text-only video generation.
- Limit each clip to **one camera move, one subject motion and one lighting change**.
- State what must remain locked: geometry, identity, material, camera axis and palette.
- Ask for a loop explicitly and define how the final state returns to baseline.
- Prefer 5-8 second loops. Longer clips increase drift and file size.
- Generate at the intended aspect ratio. Avoid cropping a portrait generation into desktop landscape.
- Do not generate typography in video. Overlay all copy in HTML.
- Do not use AI interpolation to fake scroll-linked state changes. Build the state logic with GSAP.
- Use crossfades between visually related loops instead of prompt-based object metamorphosis.
- Avoid motion presets that overpower the scientific tone, including free fall, explosions, zombie movement, paparazzi and exaggerated action effects.

### 12A.15 Sound strategy

Sound is optional. The default portfolio experience should be silent.

Appropriate uses:

- A clearly labelled `Play 15-second reel` control in the hero
- A user-triggered Sentinel or SEIL case-study film
- A social teaser exported separately from the website
- Very subtle UI feedback after the user enables sound

Do not use:

- Autoplay music
- Continuous ambient drones across the page
- Sound triggered by ordinary scrolling
- Voiceover on every chapter
- Synthetic keyboard, stock ticker or hospital-monitor clichés

**Optional 15-second sonic identity prompt for Seed Audio 1.0:**

```text
Create a 15-second restrained cinematic sound bed for a scientific and technical portfolio.
Begin with a soft physical room tone and a faint glass resonance. Introduce three precise sonic
motifs in sequence: a delicate molecular click pattern, a low-amplitude electrical pulse and a subtle
paper-and-data rhythm. Resolve them into one warm, confident tonal chord. Premium museum-installation
sound design, clean stereo image, no melody that resembles an existing work, no voice, no dramatic
trailer boom, no heartbeat, no hospital monitor, no cyberpunk bass, no aggressive riser. Leave a
clean tail for looping or fading.
```

Export audio as AAC for MP4 and Opus for WebM. Provide a visible mute control and remember the user's choice only after interaction.

### 12A.16 FFmpeg installation on macOS

FFmpeg's official site distributes source code and links to compiled macOS builds. For a Mac development workflow, the simplest route is Homebrew:

```bash
brew install ffmpeg
ffmpeg -version
ffprobe -version
```

Do not clone and compile the FFmpeg source repository unless a specific codec or build flag requires it.

### 12A.17 FFmpeg web-video pipeline

Create one reproducible script, for example `scripts/process-portfolio-media.sh`.

**Trim a generated clip to six seconds and remove generated audio:**

```bash
ffmpeg -i input.mp4 -t 6 -an \
  -vf "scale=1920:-2:flags=lanczos,fps=30" \
  -c:v libx264 -preset slow -crf 20 -pix_fmt yuv420p \
  -movflags +faststart hero-master.mp4
```

**Create a WebM version:**

```bash
ffmpeg -i hero-master.mp4 -an \
  -c:v libvpx-vp9 -crf 31 -b:v 0 -row-mt 1 \
  -deadline good -cpu-used 2 hero-loop.webm
```

**Create a high-quality poster frame:**

```bash
ffmpeg -ss 00:00:01.000 -i hero-master.mp4 -frames:v 1 \
  -vf "scale=1920:-2:flags=lanczos" hero-poster.png
```

Convert the poster to AVIF using an image pipeline such as Sharp or an FFmpeg build with AVIF support.

**Crossfade two generated chapter clips:**

```bash
ffmpeg -i biology.mp4 -i neuro.mp4 \
  -filter_complex "[0:v]trim=0:6,setpts=PTS-STARTPTS[v0]; \
                   [1:v]trim=0:6,setpts=PTS-STARTPTS[v1]; \
                   [v0][v1]xfade=transition=fade:duration=0.8:offset=5.2[v]" \
  -map "[v]" -an -c:v libx264 -crf 20 -preset slow \
  -pix_fmt yuv420p -movflags +faststart transition.mp4
```

**Normalise optional audio for a reel:**

```bash
ffmpeg -i reel-video.mp4 -i sonic-identity.wav \
  -filter_complex "[1:a]loudnorm=I=-16:TP=-1.5:LRA=8[a]" \
  -map 0:v -map "[a]" -c:v copy -c:a aac -b:a 192k \
  -shortest reel-with-audio.mp4
```

### 12A.18 Website delivery pattern

Use both WebM and MP4 with a static poster:

```html
<video
  class="chapter-media"
  muted
  loop
  playsinline
  preload="none"
  poster="/media/hero/hero-poster.avif"
  aria-hidden="true"
>
  <source src="/media/hero/hero-loop.webm" type="video/webm" />
  <source src="/media/hero/hero-loop.mp4" type="video/mp4" />
</video>
```

Runtime rules:

- Do not preload every video.
- Start loading when a chapter is within approximately one viewport.
- Pause video when it leaves the viewport.
- On `prefers-reduced-motion`, do not autoplay. Show the poster.
- On data-saver or slow connections, prefer the poster.
- Keep chapter loops below approximately 2-4 MB where visual quality allows.
- The hero poster and text must paint before hero video playback begins.
- Generated video elements are decorative and should use `aria-hidden="true"`.

### 12A.19 Suggested purchasing decision

Higgsfield is a sensible single platform for this production because it currently exposes Nano Banana Pro, Kling 3.0, Seedance 2.0, audio tools and MCP/CLI access in one environment. However, a countdown discount should not determine the design. Before paying, verify the checkout page for:

- Which models are genuinely unlimited and for how many days
- Whether unlimited use is subject to relaxed queues or fair-use limits
- Monthly credit renewal and rollover terms
- Commercial-use terms for the chosen plan
- Maximum output resolution and watermark rules
- Cancellation and renewal price after the promotion

For this portfolio, one focused month is likely enough if the scene prompts and asset ledger are prepared before generation. Generate and approve the still system first, then spend video credits only on the six to eight selected loops.

### 12A.20 Agent prompt for Higgsfield asset production

```text
You are the visual-production director for Jack Sangster's portfolio redesign.

Read:
- docs/portfolio-redesign/DESIGN.md
- docs/portfolio-redesign/MOTION.md
- docs/portfolio-redesign/STORYBOARD.md
- docs/portfolio-redesign/ASSET-DIRECTION.md
- every approved scene specification

Goal:
Create a coherent set of photorealistic scientific-editorial chapter assets using Higgsfield.
The assets support a GSAP-driven website. They do not contain factual charts, labels, EEG traces,
chemical strings, architecture diagrams or interface text.

Workflow:
1. Establish a three-image reference board for material, palette and hero geometry.
2. Generate still candidates before motion.
3. Use Nano Banana Pro for final stills.
4. Use Kling 3.0 for 5-8 second controlled image-to-video loops.
5. Use Seedance 2.0 only for an approved multi-shot reel or a sequence needing native audio.
6. Keep one camera move, one subject movement and one lighting change per loop.
7. Preserve negative space for live HTML typography.
8. Produce 16:9 desktop masters and verify mobile-safe crops.
9. Return generation prompts, model settings, selected outputs and rejected-output reasons.
10. Do not modify the website or invent project claims.

For every output report:
- asset ID
- purpose
- model
- aspect ratio
- source references
- full prompt
- negative constraints
- motion prompt if relevant
- factual elements intentionally excluded
- desktop crop result
- mobile crop result
- loop stability assessment
- approval recommendation
```

### 12A.21 Source notes, verified 1 July 2026

- Higgsfield Nano Banana Pro prompt guide: recommends explicit subject, composition, action, style, lighting and negative constraints.
- Higgsfield Kling 3.0 page: describes reference consistency, up to 15-second generation and multi-shot support.
- Higgsfield Seedance 2.0 page: describes multimodal references, multi-shot generation, native audio and clips up to 15 seconds.
- Higgsfield MCP documentation: describes access to image and video models through Claude-compatible MCP workflows.
- FFmpeg official download page: distributes source and links to macOS builds; FFmpeg remains the deterministic local stage for conversion and compression.


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
