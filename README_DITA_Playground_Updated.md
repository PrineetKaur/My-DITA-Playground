# DITA Playground

This repository is a personal learning and practice space for understanding
**DITA (Darwin Information Typing Architecture)** and structured technical
documentation.

The goal of this playground is not to showcase a finished product, but to
demonstrate **progressive learning**: starting from core concepts and
gradually moving toward more advanced DITA features and publishing workflows.

Each project in this repository is intentionally scoped and added incrementally.

------------------------------------------------------------------------

## Repository structure (project progression)

If you are new to DITA, start from the beginning and follow the folders in order:

- **`00-understanding-dita`**  
  A plain-language introduction to DITA fundamentals, written for readers who
  may not have prior experience with structured authoring.

- **`01-hello-dita`**  
  A basic DITA project that introduces core topic types (concept, task,
  reference) and shows how topics are assembled using a DITA map.

- **`02-reuse-demo`**  
  Demonstrates content reuse using DITA mechanisms such as conrefs and keyrefs,
  and explains why modular documentation matters.

- **`03-sample-product-docs`**  
  A small but realistic documentation set for a fictional product, showing how
  multiple guides can be assembled from reusable topics.

- **`04-conditional-text`**  
  Examples of conditional content for different audiences and platforms
  (for example, user vs. admin or web vs. mobile) using profiling attributes.

- **`05-dita-ot-plugin`**  
  An introductory look at DITA Open Toolkit (DITA-OT) customization, including
  a beginner-friendly plugin structure and a simple HTML output customization.

Each folder contains its own README explaining learning goals, scope, and design
decisions.

------------------------------------------------------------------------

## What this repository teaches (high-level learning outcomes)

By completing the projects in order, you will learn how to:

- Write structured content based on **user intent**
- Build reusable documentation using **modular topics**
- Assemble deliverables using **DITA maps**
- Reduce duplication using **reuse mechanisms**
- Support multiple outputs using **conditional / profiled text**
- Understand the publishing step using **DITA Open Toolkit**
- Recognize how DITA scales in real product documentation environments

The emphasis is on *clarity, structure, and reasoning* rather than completeness.

------------------------------------------------------------------------

## Prerequisites (optional but recommended)

You can read and learn from the DITA source files directly without installing
anything.

To generate published output (HTML), it helps to have:

- **DITA Open Toolkit (DITA-OT)** installed locally
- A code editor such as **VS Code**
- Basic comfort with the command line (optional, but useful)

------------------------------------------------------------------------

## How to run / publish output (DITA-OT)

You can generate HTML output from any `.ditamap` file in this repository using
DITA-OT.

Example command:

```bash
dita -i <map-file>.ditamap -f html5 -o out
```

Example (Project 03):

```bash
dita -i 03-sample-product-docs/product-docs.ditamap -f html5 -o out
```

This generates an `out/` folder containing the published HTML output.

### Project 05 plugin note
Project **05-dita-ot-plugin** also includes a beginner-friendly plugin structure.
If you want to test it fully, copy the plugin folder into your local DITA-OT
plugins directory and run:

```bash
dita --install
```

Then build output as usual:

```bash
dita -i 05-dita-ot-plugin/sample.ditamap -f html5 -o out
```

------------------------------------------------------------------------

## Why this repository exists

This playground focuses on:

- Understanding **structured authoring principles**, not just DITA syntax
- Writing documentation based on **user intent**
- Exploring **content reuse and scalability**
- Learning how DITA supports automation and multi-channel publishing
- Building a clear learning path that reflects real documentation team workflows

This repository is intentionally designed as a learning journey that can be
reviewed folder-by-folder.

------------------------------------------------------------------------

## About the approach

- Projects are intentionally small and focused
- Advanced features are introduced only after fundamentals are clear
- Each folder represents a learning milestone
- Git history reflects a gradual progression over time

This mirrors how structured documentation is learned and applied in real-world teams.

------------------------------------------------------------------------

## Ideas for future progression (for forks and further learning)

If you fork this repository and want to extend it after Project 05, here are
some realistic next milestones:

- Add **more advanced reuse patterns**
  - topicrefs with keys
  - keyscopes for multi-product documentation
  - glossary reuse

- Expand the product documentation set (Project 03)
  - add troubleshooting topics
  - add FAQ topics
  - add onboarding vs advanced user sections

- Add structured documentation quality improvements
  - consistent metadata
  - short descriptions for topics
  - basic terminology standards

- Add PDF publishing exploration
  - generate PDF via DITA-OT PDF plugins or processors
  - document challenges and decisions

- Add build automation
  - include a simple build script (bash or batch)
  - document how a documentation pipeline could run in CI

------------------------------------------------------------------------

## Notes

This repository uses fictional examples and simplified content for learning
purposes. It is not intended to represent production documentation.
