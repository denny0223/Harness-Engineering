# AGENTS.md

This repository is a Marp slide deck. Treat it as a communication artifact first and a Markdown project second. The goal is not merely to make slides render; the goal is to preserve and improve a talk that has an argument, an audience, a rhythm, and evidence.

These instructions are intentionally reusable across Marp-based slide projects. Do not overfit changes to the current deck unless the user explicitly asks for deck-specific work.

## Working Model

Approach each deck like a concise research presentation:

- Identify the central thesis before editing individual slides.
- Understand the audience, their prior knowledge, and what should change in their mind after the talk.
- Preserve the line of reasoning: motivation, context, evidence, interpretation, implication, and closure.
- Treat each slide as one move in an argument, not as an isolated Markdown fragment.
- Prefer clarity, sequence, and visual economy over decorative complexity.
- Distinguish claims, evidence, examples, citations, and speaker prompts.

When the deck is about an organization, community, product, research topic, or historical narrative, avoid flattening it into a timeline. A good deck explains why events matter, what changed, and what the audience should infer.

## Editing Principles

- Keep edits scoped to the user request and the deck's existing style.
- Do not rewrite the author's voice unless the request is explicitly about tone, structure, or narrative.
- Improve slide flow by reducing ambiguity, strengthening transitions, and removing accidental redundancy.
- Prefer one strong idea per slide. If a slide carries multiple claims, split it or make the hierarchy explicit.
- Avoid turning slides into prose documents. Speaker context can exist in notes or adjacent structure, but on-slide text should remain sparse.
- Preserve intentional pacing slides, title-only slides, full-bleed image slides, and pause slides unless they clearly break the requested goal.
- Keep terminology consistent across the deck, especially names, dates, roles, project titles, and recurring concepts.
- When adding factual claims, verify them from reliable sources or mark assumptions clearly for the user.
- When editing dates, statistics, event names, or attributions, prefer exactness over rhetorical convenience.

## Narrative And Argument Quality

Use the same standards expected in strong academic and technical talks:

- Every major claim should have a visible basis: data, example, source, lived evidence, or a clear warrant.
- The deck should make scope conditions clear. Avoid universal claims when the evidence is local, historical, or anecdotal.
- Avoid unexplained jumps between abstraction levels. If moving from a concrete example to a general principle, make the bridge legible.
- Introduce specialized terms before relying on them.
- Keep the audience's cognitive load low: one conceptual shift at a time, clear grouping, and minimal competing visual signals.
- Use contrast deliberately: before/after, problem/response, myth/reality, principle/example, local/global.
- End sections with synthesis, not just the next topic.

If a requested edit weakens the argument, explain the tradeoff briefly and propose a sharper alternative before making broad structural changes.

## Marp Conventions

- The primary source is usually `slide.md`. Edit generated output such as `index.html` only when the user explicitly asks for output-file changes.
- Keep YAML front matter valid and minimal. Do not add project-specific metadata unless it serves the deck or publishing workflow.
- Use `---` for slide boundaries. Preserve Marp directives, comments, and slide-local classes unless changing them is part of the task.
- Prefer Marp-native image syntax for simple slides and HTML only when Marp syntax cannot express the layout cleanly.
- Keep custom CSS small, purposeful, and close to the deck's established visual system.
- Do not introduce a build system, package manager, theme framework, or asset pipeline unless the repository already uses one or the user asks for it.
- If scripts exist, prefer existing scripts over new commands. If no scripts exist, use the simplest Marp-compatible validation available in the environment.

## Visual And Media Standards

- Visuals should carry meaning, not merely decorate.
- Maintain image aspect ratios unless cropping is intentional.
- For full-bleed images, verify that the important subject is not hidden by slide text, pagination, or viewport cropping.
- Prefer stable local assets in the repository for repeatable builds.
- When adding external media embeds, consider offline behavior, privacy, accessibility, and whether the deck still communicates when the embed fails.
- Keep image filenames descriptive and durable.
- Preserve license and attribution information for reused assets.

## Language And Tone

- Match the deck's language. If the deck is in Traditional Chinese, keep user-facing slide text in Traditional Chinese unless asked otherwise.
- This instruction file is in English because it is primarily for coding agents.
- Keep slide copy concise, concrete, and speakable.
- Avoid generic marketing phrasing, inflated claims, and filler.
- Prefer active, direct phrasing when it improves comprehension.
- Preserve culturally specific terms, community names, and proper nouns carefully.

## Accessibility And Presentation Quality

- Ensure headings are readable from a distance.
- Avoid dense lists unless the slide is meant to be scanned as a reference.
- Watch for long lines, cramped text, low contrast, and overlapping elements.
- Use visual hierarchy consistently: title, subtitle, evidence, source, and aside should not compete equally.
- When possible, make links human-readable and preserve target URLs.
- Do not rely on color alone to communicate meaning.

## Verification

Before finishing a change:

- Review the diff for unintended generated-file churn.
- Check that Markdown, front matter, slide separators, HTML tags, and Marp directives remain well formed.
- If a Marp build or preview command exists, run it.
- If no build command exists, at least inspect the edited source around every changed slide.
- For visual/layout changes, prefer rendering or previewing the deck when the environment supports it.
- Report any validation you could not run and why.

## Collaboration With The User

- For small textual or structural fixes, make the change directly.
- For broad narrative restructuring, first state the proposed structure and the reasoning.
- For factual additions, cite or summarize the evidence path used.
- If the user's request is ambiguous, infer conservatively from the deck and existing style. Ask only when the choice changes the talk's thesis, audience, or publishing workflow.
- Keep final reports short: what changed, where, and how it was checked.

