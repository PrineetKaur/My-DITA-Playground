# Understanding DITA (in simple terms)

DITA (Darwin Information Typing Architecture) is a way of writing technical documentation that forces writers to separate content by user intent.

Instead of writing long documents that mix explanations, instructions, and tables, DITA encourages writing small, focused topics that can be reused and assembled in different ways.

At its core, DITA separates documentation into three main types of content:

## 1. Concept – What is this?
Concept topics explain what something is, why it exists, and how it fits into the bigger picture.

Examples:
- What is this product?
- What problem does it solve?
- How does it work at a high level?

Concept topics provide background and context. They do not include step-by-step instructions.

## 2. Task – How do I do this?
Task topics describe how to perform a specific action.

Examples:
- How to install the product
- How to configure authentication
- How to deploy a service

Task topics are procedural and focus on clear, ordered steps.

## 3. Reference – What are the details?
Reference topics provide factual, structured information that users look up while working.

Examples:
- Command options
- API parameters
- Configuration values

Reference topics are optimized for scanning, not for narrative reading.

## Why this separation matters
Separating content by intent:
- Makes documentation easier to reuse
- Reduces duplication
- Improves consistency
- Scales better for large products
- Works well with automation and AI-assisted tooling

This repository uses these principles throughout the examples that follow.
