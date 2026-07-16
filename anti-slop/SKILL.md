---
name: anti-slop
description: Detect and flag AI slop patterns in any piece of writing. Use this skill whenever the user wants to check a draft for AI-sounding language, generic phrases, or robotic patterns. Trigger on phrases like "check this for AI slop", "does this sound AI-written", "slop check", "flag the AI patterns", "is this too AI-ish", "make this sound less robotic", "audit my writing", or when the user pastes a draft and asks if it sounds human. Also trigger proactively when reviewing any piece of copy, content, or written draft where the user seems concerned about voice or authenticity. The skill analyzes writing against the 21 patterns in the Anti-AI Slop Playbook and returns a structured report with flagged lines and specific fixes.
---

# Anti-AI Slop Detector

You are a writing auditor trained on the Complete Anti-AI Slop Playbook. Your job is to read submitted writing and flag every pattern that makes it sound AI-generated, then return a clear report with specific fixes.

## Reference

Before analyzing, read the full playbook at:
`references/playbook.md`

This contains all 21 patterns organized into 4 parts:
- Part 1: Structural Red Flags (Red Flags 1-6)
- Part 2: Formatting Giveaways (Red Flags 7-9)
- Part 3: Phrase Patterns That Scream "Robot" (Patterns 1-9)
- Part 4: Content Red Flags (Red Flags 10-12)

## How to Run the Audit

### Step 1: Read the draft fully before flagging anything

Get the full picture before you start marking things up. Understand the intent, audience, and tone the writer is going for.

### Step 2: Check against every pattern in the playbook

Go through each of the 21 patterns systematically. For each one, ask: does this draft contain any instance of this pattern?

Patterns to check:

**Structural:**
1. Binary Contrast Addiction ("it's not X, it's Y")
2. Triple Threat Syndrome (groups of exactly three)
3. Infomercial Transitions ("the catch?", "want to know the secret?", "the brutal truth?", "here's the kicker")
4. Corporate Verb Disease (-ing verbs: highlighting, emphasizing, facilitating, leveraging)
5. Hedging Language ("it's worth considering", "you might want to think about", "it's important to note")
6. Thesaurus Abuse (utilize, execute, facilitate, implement, optimize, leverage)

**Formatting:**
7. Arrow Obsession (→ used repeatedly)
8. Emoji Explosion (multiple emojis used for decoration)
9. Em Dash Overdose (more than 2 em dashes per paragraph)

**Phrase Patterns:**
10. "No X. No Y. Just Z." structure
11. "Game-changer" / "supercharge" / "this changed everything"
12. "Real" Overload (real strategy, real results, real experts)
13. The Serious Pitch ("if you're serious about X, let's Y")
14. "To Your Success" sign-offs
15. Profound But Obvious ("not because of X. but because of Y")
16. Short Hook Questions ("the best part?", "want access?", "ready to level up?")
17. "Enter: [Thing]"
18. "Stopped me in my tracks" / melodramatic mentor moments

**Content:**
19. Symbol Obsession ("this symbolizes", "which reflects", "emphasizing the importance of")
20. The Generic Case Study (invented generic personas, no real names/numbers)
21. "Everything Changed" hyperbole ("changed everything", "transformed my entire business")

### Step 3: Build the report

Structure your output like this:

---

## Slop Audit: [Score] patterns flagged

**Severity:** [Clean / Minor / Moderate / Heavy]

---

### Flagged Patterns

For each flagged pattern, show:

**[Pattern Name]**
> "[exact quote from the draft that triggered this flag]"
Fix: [one specific sentence rewrite or instruction]

---

### Summary

[2-3 sentences on the overall voice. What's working. What's dragging it toward AI territory.]

### Biggest Priority

[Single most important fix they should make first.]

---

## Severity Scale

- **Clean** (0-2 flags): Strong human voice. Minor polish needed.
- **Minor** (3-5 flags): Solid draft with a few robotic patches. Quick fixes.
- **Moderate** (6-10 flags): AI patterns are noticeable. Needs a real pass.
- **Heavy** (11+ flags): Reading as AI-written. Needs significant rewrite.

## Tone Guidelines

- Be direct. Name the pattern, quote the line, give the fix.
- Don't soften feedback. The user wants to know what's wrong.
- Don't flag things that aren't in the playbook. Stick to the 21 patterns.
- If a pattern appears multiple times, flag it once with the worst example. Note how many times it appears total.
- If the draft is clean, say so clearly. Don't invent problems.
- Fixes should be specific rewrites, not vague advice like "be more specific."
File 2: anti-slop/references/playbook.md
This one has real content (the actual 21 patterns explained in depth). Let me pull that file for you next so you can create it as a second file inside the same folder.Reading the playbook reference file to hand over its content nextReading the playbook reference file to hand over its content nextThis one is also generic and ready to go as is. Here's the second file.
File 2: anti-slop/references/playbook.md
When creating this file in GitHub, type anti-slop/references/playbook.md as the filename (this creates the nested references subfolder automatically), then paste this:
markdown# The Complete Anti-AI Slop Playbook

## Part 1: Structural Red Flags

### Red Flag #1: Binary Contrast Addiction
AI can't resist the "it's not X, it's Y" structure.
- "success isn't about working hard, it's about working smart"
- "content isn't about quantity, it's about quality"
- "marketing isn't selling, it's storytelling"

Real humans don't speak in constant philosophical opposites.
**Fix:** Say what you mean directly. Use specific details instead of broad contrasts.

---

### Red Flag #2: Triple Threat Syndrome
AI learned that grouping things in threes makes "good writing." So it does it everywhere.
- "fast, efficient, reliable"
- "boost engagement, increase conversions, maximize roi"
- "powerful, simple, transformative"

**Fix:** Vary your rhythm. Sometimes use two things. Sometimes four. Sometimes just one.

---

### Red Flag #3: Infomercial Transitions
Cringe questions AI uses to create "engagement":
- "the catch?"
- "want to know the secret?"
- "the brutal truth?"
- "here's the kicker"

Sounds like a 3am cable shopping channel.
**Fix:** If you wouldn't say it in real conversation, don't write it.

---

### Red Flag #4: Corporate Verb Disease
Stuffy -ing verbs:
- "...highlighting the benefits..."
- "...emphasizing critical importance..."
- "...facilitating better outcomes..."

Nobody talks like a middle management memo.
**Fix:** Use simple, active verbs. "show" not "highlighting." "help" not "facilitating."

---

### Red Flag #5: Hedging Language
AI loves to clear its throat:
- "it's worth considering..."
- "you might want to think about..."
- "it's important to note that..."

**Fix:** State your opinion. Skip the diplomatic warm-up.

---

### Red Flag #6: Thesaurus Abuse
Fancy words that signal AI authorship:
- "utilize" → use
- "execute" → do
- "facilitate" → help
- "implement" → start
- "optimize" → improve
- "leverage" → use

**Fix:** Write like you talk.

---

## Part 2: Formatting Giveaways

### Red Flag #7: Arrow Obsession
AI discovered the → symbol and won't let go:
→ 10x your results
→ scale faster than ever
→ join today

**Fix:** Use arrows sparingly. One per post maximum.

---

### Red Flag #8: Emoji Explosion
ChatGPT treats emojis like confetti:
- boost productivity now!
- revolutionary new approach!
- transform your business!

**Fix:** One emoji per section. Maybe. Or none.

---

### Red Flag #9: Em Dash Overdose
Yes, writers use em dashes. No, not 6 times per paragraph.
AI loves stacking multiple em dash asides in a single sentence to add caveats and flourishes.

**Fix:** Mix your punctuation. Commas exist. Periods too.

---

## Part 3: Phrase Patterns That Scream "Robot"

### Pattern #1: "No X. No Y. Just Z."
- "no fluff. no theory. just actionable insights."
- "no gimmicks. no shortcuts. just results."

**Fix:** Literally any other sentence structure.

---

### Pattern #2: "The game has changed"
Along with its cousins:
- "game-changer"
- "supercharge your [thing]"
- "this changed everything"

**Fix:** Describe actual change without hyperbole.

---

### Pattern #3: "Real" Overload
"just real strategy from real experts getting real results with real entrepreneurs."

**Fix:** Show authenticity through specific examples, not by repeating "real."

---

### Pattern #4: The Serious Pitch
"if you're serious about [goal], let's [cta]"

Every AI-written CTA uses this exact structure.
**Fix:** Vary your calls to action. Be specific about what happens next.

---

### Pattern #5: "To Your Success"
Email sign-offs like this instantly reveal AI authorship.
**Fix:** Sign off like a human. "cheers," "talk soon," or just your name.

---

### Pattern #6: Profound But Obvious
"not because of X. but because of Y"
- "i didn't succeed because of luck. but because of hard work."
- "this won't work because of the tool. but because of the user."

AI's attempt at wisdom. Usually states the obvious.
**Fix:** If everyone already knows it, don't package it as insight.

---

### Pattern #7: Short Hook Questions
- "the best part?"
- "want access?"
- "ready to level up?"

Very 2023 ChatGPT energy.
**Fix:** Ask real questions that require thought to answer.

---

### Pattern #8: "Enter: [Thing]"
"enter: my revolutionary framework"
"enter: the solution you've been searching for"

**Fix:** Just introduce the thing normally.

---

### Pattern #9: "Stopped Me in My Tracks"
"yesterday my mentor said something that stopped me in my tracks:"

Sounds like everyone's having world-altering realizations daily.
**Fix:** Describe actual impact without melodrama.

---

## Part 4: Content Red Flags

### Red Flag #10: Symbol Obsession
AI loves telling you what things "represent" instead of what happened:
- "this symbolizes..."
- "which reflects..."
- "emphasizing the importance of..."

**Fix:** Say what happened. Say what you learned. Skip the literary analysis.

---

### Red Flag #11: The Generic Case Study
When AI lacks real data, it invents people. Usually named "Sarah Chen."
**Fix:** Use actual examples from your life. Real names (with permission). Real numbers.

---

### Red Flag #12: Everything Changed
"the strategy that changed everything"
"this one shift transformed my entire business"

**Fix:** Describe specific changes with specific metrics.
