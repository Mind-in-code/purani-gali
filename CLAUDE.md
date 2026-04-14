# Project — Claude Instructions

## Mandatory: Project Memory
**ALWAYS** read `PROJECT_CONTEXT.md` at the start of every conversation. It's the single source of truth for what this project is, what's built, what's pending, and recent decisions.

**ALWAYS** update `PROJECT_CONTEXT.md` at the end of every conversation that produces new decisions, features, or changes. Add a short entry to the changelog at the bottom.

If `PROJECT_CONTEXT.md` doesn't exist yet, create it with these sections: Overview, Tech Stack, What's Built, What's Pending, Key Decisions, Changelog.

---

## Hard Rules (non-negotiable)

1. **Confirm before code changes.** Always ask before editing code. Clarify ambiguous or risky requests first. Never guess — ask.
2. **Plan before acting.** Any task with 3+ steps or an architectural decision gets a plan first. Write the plan in `tasks/todo.md` with checkable items. Wait for approval before implementing.
3. **Stop when things go sideways.** If a task isn't going as planned, STOP. Don't push forward solo. Report the blocker and ask how to proceed.
4. **Verify before marking done.** Never mark a task complete without proving it works. Run it. Check the output. Show evidence. No "it should work" — only "here's proof it works."
5. **Root causes, not band-aids.** Find the real cause of a bug. No temporary fixes. No suppressing errors to make them go away. Senior developer standards only.
6. **Simplicity first.** Make every change as simple as possible. Touch minimal code. Avoid introducing new abstractions, libraries, or patterns unless truly necessary.
7. **Minimal impact.** Changes should only touch what's necessary. Don't refactor unrelated code "while you're there."
8. **Be direct.** No corporate fluff. No "it depends" answers. Take a position and explain the reasoning. If an idea is bad, say so.

---

## Workflow

### Plan Mode Default
- Enter plan mode for any non-trivial task (3+ steps or architectural decisions)
- Write the plan in `tasks/todo.md` as checkable items
- Get approval on the plan BEFORE writing code
- Mark items complete as you go

### Self-Improvement Loop (the compounding one)
- After ANY correction from me, note the pattern in `tasks/lessons.md`
- Write a rule for yourself that prevents the same mistake next time
- Review `tasks/lessons.md` at the start of every session
- This is a compounding system — the longer you use it, the smarter it gets

### Subagents for Research
- When you need to explore multiple files, research libraries, or compare approaches, spawn subagents
- One task per subagent. Focused execution.
- Keeps the main conversation clean and the context window uncluttered

### Sprint Pattern
- Focus on ONE task at a time. Don't context-switch mid-build.
- Finish the current thing before starting the next thing
- If context gets full (~70%), compact. If it's very full (~90%), clear and re-read `PROJECT_CONTEXT.md`.

---

## Task Management

Keep two files in the project:

- **`tasks/todo.md`** — current plan for the task in progress. Checkable items. Marked complete as you go. Include a "Review" section at the bottom after the task is done summarizing what changed and why.
- **`tasks/lessons.md`** — patterns captured from corrections. Each entry: what the mistake was, why it happened, the rule to follow next time.

---

## Code Quality Standards

- **Write the simplest code that works.** Not the cleverest.
- **No laziness, no fluff.** Every recommendation should be specific, actionable, and backed by reasoning.
- **Challenge your own work.** Before presenting a solution, ask: "Is there a simpler way? Would a senior developer approve this?"
- **No generic "it depends" answers.** Take a position and defend it with reasoning.
- **Don't over-engineer.** For small, obvious fixes, skip the "is there a more elegant way?" step. Don't build frameworks when a function will do.

---

## Website Project Rules (Plain HTML/CSS/JS + Spline 3D)

- **No frameworks, no build tools.** This is vanilla HTML/CSS/JS. Don't suggest React, Vue, Tailwind, or npm. If it can't run with `python3 -m http.server`, it doesn't belong.
- **Check responsive behavior** on every UI change — test at 1024px, 768px, and 480px breakpoints
- **Verify accessibility basics** — alt text on images, aria-labels on interactive elements, form labels, keyboard navigation
- **Test in the actual browser** before marking anything complete — not just the code
- **CSS Custom Properties for all design tokens** — colors, fonts, and easing are defined in `:root`. Use the variables, don't hardcode hex values.
- **Inline SVG for logos** — never use `<img>` tags for the Purani Gali logo. Always inline the SVG for crisp rendering and transparency.
- **Spline embeds are iframes** — don't try to manipulate Spline scenes via JS. Interactive ones get `pointer-events: auto`, ambient backgrounds get `pointer-events: none`.
- **Keep it zero-dependency** — no jQuery, no libraries. Canvas API for particles, IntersectionObserver for animations, vanilla event listeners for everything else.
- **Respect `prefers-reduced-motion`** — all animations and transitions must degrade gracefully
