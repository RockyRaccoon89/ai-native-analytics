# Context
## Ideas to structure into the book
- Context file
    - repo centric
        - repo architecture
    - team centric
        - coding standards
        - documentation standards
        - coding process
        - paterns
- Product Specification
    - use case: context and value. who, goal & business outcome
        - should never use system language
        - stay in business language, focused on user goal and value
        - If a technical term is unavoidable and widely understood, you can include it, but only to clarify context, not to prescribe design.
    - implementation plan: exact system change
        - implementation plan should be link the request
        - build from standards and document exception and their justification from standards
        - ? ephemerous - once the work is completed, should be archived
    - Requirements: what capability must exist
        It defines what the solution must do, what rules it must respect, and how success is measured.
    - data contract
        - data contract enforcement
- skill areas
    - groupment of skills
    - naming structure: area.skill ex:
        - documentation.erd
        - documentation.readme
- skills
    - like a function
    - "teach" the skill. Do the work then ask the AI to create the skill to reproduce the work that was done. 
    - **must** be embeed in process
        - assure value
        - increase learning
        - also mean that need to standardize process
    - skill structure
        - should be small enough to be tester and reuse.
            - most skill are really big
            - need to be small enough to be tester
        - ? modules?
    - A skill is the equivalent of an how-to
        - Like a good how-to, it can be use to standardize, optimize and continuous improvement
    - need to implement RACI & continuous improvement processes
        - define the feedback loop
        - skill versionning
    - skill can not only produce a standardized output but also safeguard againts previous pitfalls
    - type of skill
        - support
            - profiling: AI to show data & exception and the dev manually provide the correct output
                - ? how to be cost effective
                - ? directly link with use case
            - control on standards
            - control on governance (ex: proper approbation)
        - build
            - build & maintain implementation plan
            - help generate data test
                - would support "data test coding"
            - transformation: provide data test & standards and get transformation
            - documentation
                - from use case
                - from implementation
    - should not be managed inside the code base
        - Governance missmatch: code is manage for what it does with it's own RACI while the skills should be manage in it's own governance process. Ex: change in a skill used internally to the team shouldn't need CAB approval
        - some skills could be reused from different repo
        - missmatch between what is in the repo and what the code does. this will happen if the skills are updated but the code doesn't change
- D&A processes with AI
    - human process & skill processes interconnection
    - to leverage the AI the processes must be more mature
        - need better request documentation to feed the AI
        - need better code base and use case documentation to avoid regression on already existing objects
        - need structure
            - Reference information (context files & standards)
            - Reference process (skill)
- Team impact
    - Role change
    - Training - upskilling


## Chapters

### Introduction
- Why this book exist
- Why should you read it
- How to read this book
- Why should you contribute

### Chapter 1: AI Needs Structure More Than You Think
The promise is simple: AI helps you build faster. The catch? It can only be as good as the structure around it. This chapter sets the stage, not just about tools, but about how human processes and AI processes interconnect. They don't run side by side; they feed each other. Leveraging AI in analytics demands more mature processes: better request documentation, better codebase and use case documentation to avoid regressions, and a clear separation between reference information (context files, standards) and reference processes (skills). Every chapter that follows builds on this interconnection.

Ideas covered:
- The interconnection between human processes and AI skill processes
- Why leveraging AI demands more mature processes
- The need for better request documentation to feed the AI
- The need for better codebase and use case documentation to prevent regressions
- The two pillars of structure: reference information (context files, standards) and reference processes (skills)

### Chapter 2: Giving the AI Something to Work With — Context Files
AI doesn't know your team. It doesn't know your repo architecture, your coding standards, or how you like your documentation. Context files fix that. This chapter introduces two flavors: repo-centric context (your repository architecture) and team-centric context (coding standards, documentation standards, coding process, and patterns). Together, they form the reference information the AI draws from to produce work that actually fits.

Ideas covered:
- Context files as the foundation of AI-assisted work
- Repo-centric context: repository architecture
- Team-centric context: coding standards, documentation standards, coding process, and patterns

### Chapter 3: From Request to Action — Use Cases and Workplans
Work starts with a use case. A workplan turns it into a concrete system change. This chapter walks through that lifecycle: how the workplan links back to the request, how it builds from established standards (and documents any justified exceptions), and why the workplan is ephemerous — once the work is done, it gets archived, not preserved as permanent documentation.

Ideas covered:
- The use case: who it serves, the goal, and the business outcome
- Writing in business language, never in system language (technical terms only to clarify context, not to prescribe design)
- The implementation plan as the exact system change, linked to the request
- Building from standards and documenting justified exceptions
- The ephemerous nature of the implementation plan (archived once work is completed)
- Requirements: what the solution must do, what rules it respects, how success is measured
- Data contracts and their enforcement

### Chapter 4: What Is a Skill (and Why It Matters)
A skill is like a function. It's the equivalent of a how-to guide — one that can be used to standardize, optimize, and continuously improve. This chapter introduces what skills are and the two types that matter:

- **Support skills**: Profiling (the AI surfaces data and exceptions, the developer provides the correct output), control on standards, and control on governance (e.g., proper approbation).
- **Build skills**: Building and maintaining workplans, generating data tests (supporting "data test coding"), transformation (provide data test and standards, get transformation), and documentation (from use case, from workplan).

A skill doesn't just produce consistent output — it also safeguards against previous pitfalls.

Ideas covered:
- A skill works like a function and reads like a how-to guide
- Skills standardize output and safeguard against previous pitfalls
- Teaching the skill: do the work first, then ask the AI to reproduce it as a skill
- Skills must be embedded in process (assures value, increases learning, standardizes work)
- Support skills: profiling, control on standards, control on governance
- Build skills: implementation plans, data test generation, transformation, documentation
- Open questions: cost effectiveness, direct link with use case
- Skill areas as groupings with a naming convention (area.skill)
- Why skills should not live inside the codebase (governance mismatch, cross-repo reuse, repo-vs-code drift)
- Skill structure: small enough to test and reuse (modules as a potential solution)
- RACI, continuous improvement, feedback loops, and skill versioning

**Concept diving**
- "Teaching" the skill: You do the work first, then ask the AI to create the skill to reproduce what you did.
- Skills **must** be embedded in process. That's how they assure value, increase learning, and push toward standardized processes.
- Skills should not be managed inside the codebase. Code is managed for what it does, with its own RACI. Skills need their own governance process. A change in a skill used internally to the team shouldn't need CAB approval. Some skills are reused across different repos. And when skills are updated but the code doesn't change, managing them together creates a mismatch between what's in the repo and what the code actually does.

**Technical details**
- Skill structure: small enough to be tested and reused. Most skills today are too big. Modules might help.
- RACI and continuous improvement processes for managing skills over time.

### Chapter 5: Making It All Work Together
Chapter 1 introduced the interconnection between human and AI processes. Each chapter since has shown a piece of it — context files feeding the AI's understanding, workplans bridging requests to action, skills embedding AI into daily work. This closing chapter brings those pieces together: how context files as reference information and skills as reference processes form a coherent system, and what it looks like when the loop is working end to end.

Ideas covered:
- Full synthesis of the human process and skill process interconnection
- The complete structure in action: reference information (context files, standards) combined with reference processes (skills)

# Goal
1. The goal of this workplan is to take the chapter structure and information and create the relevant artefact in the code base.
2. The chapter_x.md file should be created and have the information created in the current document added as reference.
3. The SUMMARY.md must be updated with the relevant information

# Workplan

## Step 1: Create chapter files
Create the following files under `src/`:

| File | Content source |
|------|---------------|
| `src/introduction.md` | Update existing file with: Why this book exists, why you should read it, how to read this book, why you should contribute |
| `src/chapter_1_ai_needs_structure.md` | Update existing file (rename from chapter_1.md) with Chapter 1 description and ideas covered |
| `src/chapter_2_context_files.md` | Create with Chapter 2 description and ideas covered |
| `src/chapter_3_use_cases_and_workplans.md` | Create with Chapter 3 description and ideas covered |
| `src/chapter_4_skills.md` | Create with Chapter 4 description, ideas covered, concept diving, and technical details |
| `src/chapter_5_making_it_all_work.md` | Create with Chapter 5 description and ideas covered |

Each file should contain:
- The chapter title as an H1
- The chapter description as introductory text
- The "Ideas covered" list as a reference section for future writing

## Step 2: Update SUMMARY.md
Replace the current `src/SUMMARY.md` content with:

```markdown
# Summary

- [Introduction](./introduction.md)
- [AI Needs Structure More Than You Think](./chapter_1_ai_needs_structure.md)
- [Giving the AI Something to Work With — Context Files](./chapter_2_context_files.md)
- [From Request to Action — Use Cases and Workplans](./chapter_3_use_cases_and_workplans.md)
- [What Is a Skill (and Why It Matters)](./chapter_4_skills.md)
- [Making It All Work Together](./chapter_5_making_it_all_work.md)
```

## Step 3: Validate
- Confirm all files exist under `src/`
- Confirm `SUMMARY.md` links match actual filenames
- Confirm the book builds without errors (`mdbook build`)