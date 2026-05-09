# ai-native-analytics
An open-source guide to designing analytics systems for AI-assisted development

## License

Content in this repository is licensed under the Creative Commons Attribution-ShareAlike 4.0 International License (CC BY-SA 4.0).

Code examples and scripts are licensed under the MIT License.

# How to contribute

This project is a book. Changes should improve both technical accuracy and reading flow across chapters.

### 1) Before opening an issue
- Check existing Discussions and Issues for related proposals.
- If your idea changes book structure or chapter sequencing, start with a Discussion first.
- If your idea is a scoped fix or addition, open an Issue directly.

### 2) Open a high-quality issue
At minimum, include:
- Problem: what is unclear, missing, or incorrect.
- Proposed change: what should be added or edited.
- Scope: which chapters/files are affected.
- Why now: impact on readers or maintainability.
- Acceptance criteria: what "done" looks like.

### 3) Triage and backlog
- The editor reviews new issues and may:
	- accept to backlog,
	- request clarification,
	- or close with rationale.
- Structural proposals may require Discussion consensus before backlog.

### 4) Implementation workflow
- Work only on issues in backlog.
- Create a branch linked to that issue.
- Keep changes focused to one issue whenever possible.
- Update related sections when a change affects narrative continuity.

### 5) Pull request requirements
Your PR should include:
- Link to the issue.
- Summary of what changed and why.
- List of affected chapters/files.
- Notes on trade-offs or alternatives considered.
- Screenshots/output only if relevant to examples.

### 6) Review expectations
- Reviews prioritize coherence, technical correctness, and chapter flow.
- The editor sets final direction and may request restructuring for consistency.
- Approved PRs are merged when acceptance criteria are met.

### 7) Issue tags
To keep triage and planning consistent, use the following tags on issues.

Required tags:
- Exactly one `type/*` tag.
- Exactly one `priority/*` tag.
- At least one `scope/*` tag.

Type tags (pick one):
- `type/content`: chapter content, explanations, examples.
- `type/structure`: chapter order, section movement, table of contents flow.
- `type/quality`: clarity, consistency, terminology, narrative coherence.
- `type/fix`: factual errors, broken links, incorrect code snippets.
- `type/meta`: repository process, templates, contribution docs.

Priority tags (pick one):
- `priority/p0`: critical correctness issue or high reader impact.
- `priority/p1`: high impact and should be handled in the next cycle.
- `priority/p2`: normal planned work.
- `priority/p3`: nice-to-have improvement.

Scope tags (pick at least one):
- Use chapter-based tags such as `scope/introduction`, `scope/chapter-1`.
- Use multiple `scope/*` tags when an issue affects more than one section.

Tagging rules:
- If an issue has more than one possible `type/*`, choose the primary intent.
- PRs should inherit `type/*`, `priority/*`, and `scope/*` from their linked issue.
- Issues missing required tags may be sent back for clarification before backlog.

# Guide of style

Our style is clear, direct, and reader-friendly. Here’s how to keep your writing on target:

- Be straightforward. Say what you mean, skip the fluff, and get to the point.
- Use jargon only when it truly helps the reader (for example, when a technical term is widely known and makes things clearer or more precise). If you must use a less common term, give a quick definition.
- Don’t be afraid to have a little fun! A clever turn of phrase or a light joke is welcome, as long as it doesn’t distract or undermine professionalism.
- Stay professional. Avoid sarcasm, inside jokes, or anything that could be misunderstood.
- Prefer short sentences and active voice. Make your writing easy to scan and understand.
- Use examples and analogies when they help clarify complex ideas.
- Don’t take yourself (or the project) too seriously—just take the reader’s time seriously.
- Consistency matters: follow the structure and terminology already used in the book unless you have a good reason to change it.

In short: Write for humans. Make it accurate, approachable, and enjoyable to read.

# Book structure

The book is structured into three complementary tracks to balance readability, depth, and technical precision. Each track serves a distinct purpose:

## Main content
This is the core narrative of the book. It introduces the key concepts and explains their relationships in a way that can be read independently. The focus is on clarity and flow, making it accessible to a broad audience.

**Example content:** An overview of AI-native analytics systems, their components, and how they interact.

## Concept diving
Some concepts are rich enough to warrant deeper exploration, but including too much detail in the main track would disrupt readability. These deeper dives expand on the high-level explanations in the main content, providing additional context and nuance.

**Example content:** A detailed exploration of dependency management in AI systems, building on its introduction in the main content.

## Technical details
This track is for the nitty-gritty specifics. It covers tools, templates, job descriptions, architecture patterns, and other highly detailed topics. The tone is factual and professional, similar to a Wikipedia article, with clear distinctions between facts and opinions.

**Example content:** A comparison of popular tools for AI data pipelines, or a working template for designing an AI-native dashboard.

### How to use the tracks
- **Readers:** Start with the Main content to understand the big picture. Dive into Concept diving or Technical details as needed for more depth or practical guidance.
- **Contributors:** Ensure your content fits the purpose of the track you're contributing to. Keep the Main content concise, use Concept diving for rich explanations, and reserve detailed specifics for the Technical details track.

# Use of AI tools for writing

Not everyone is a natural-born wordsmith, but that shouldn’t stop you from sharing great ideas. Large Language Models (LLMs) are fantastic for polishing your writing—when used thoughtfully. Here’s how to get the most out of AI tools in this project, with some friendly do’s and don’ts.

## Principles
- The thinking is up to you—AI is here to help, not to replace your brain.
- No “text dumping.” If it reads like a wall of AI-generated text, it’s out.
- Always review and fact-check AI output. If it can be verified, verify it.

## Do
- Point your AI tool to the Guide of style for a consistent voice. If you find yourself constantly fixing the style, consider suggesting improvements to the Guide.
- Start by writing what you want to say, in your own words. Don’t worry about grammar, structure, or even language—just get your ideas down. (If English isn’t your first language, draft in your native tongue and translate later.)
- Once you’re happy with your draft, ask your AI tool to review it. Use its feedback to spot strengths and weaknesses, then apply your own judgment to improve the text. Finally, let the AI help you polish the writing to match the Guide of style.

## Don’t
- Don’t ask the AI to write a section from scratch without giving it your own draft first.
- Don’t use AI to write or rewrite large parts of the book in one go. That creates monster pull requests and dumps the responsibility for thinking and editing onto reviewers.