🔹 What is SPECKit Plus? – Write a short note.


Spec-Kit Plus is a spec-driven development framework that helps developers build software using clear written specifications. Instead of starting with code, you first write a spec, and then the framework (with the help of an AI tool) generates code, plans, tasks, and documentation from that spec.

It provides ready-made templates, commands, and a project structure that makes development more organized. The main goal of Spec-Kit Plus is to create high-quality, well-structured projects where both the code and the reasoning behind the code (plans, decisions, specs) are saved and reusable.

1. /constitution

Creates a “project constitution” — a document that defines immutable, project-wide rules and standards (coding style, architecture constraints, security/accessibility standards, team conventions, etc.). 

This constitution applies globally to all features: it ensures that every subsequent spec, plan, task or code respects the same baseline rules

2. /specify

Used to define what you are building and why — not technical details but product-level requirements: user stories, desired behavior, user experience, motivations, success criteria. 

It generates a full specification (spec) document (often a PRD-style doc) that becomes the source of truth for the feature.

3. /plan

Once the spec (what) is defined, /plan defines how to build it technically: which frameworks/libraries/technologies to use, architecture decisions, constraints, infrastructure, dependencies, etc. 
The output is a “plan” document (plan.md or similar) that ties together the spec with the project-wide constitution, ensuring technical decisions align with the established rules

4. /tasks

Converts the spec + plan into a detailed task list — breaking down the work into small, manageable, sequential (or parallel) tasks. 

Each task is a concrete actionable item (e.g. “create authentication endpoint”, “write component X”, “add tests for Y”), often with dependencies, file paths, and testing instructions. 
Basically transforms abstract requirements into a “to-do roadmap” that is easy for you or an AI to implement systematically.

5. /implement

This is the execution step: given the tasks list, the AI (or system) carries out the tasks — generating code, creating files, wiring components, installing dependencies etc. 
Because everything is backed by constitution → spec → plan → tasks, the implementation is much more controlled, traceable, and aligned with expectations, reducing guesswork and misinterpretation by the AI.