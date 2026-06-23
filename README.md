# Sally Wieland — Portfolio

Personal portfolio site. Multi-page (homepage + case study pages), deployable static HTML/CSS, no build step.

## Status
- `index.html` — homepage. Copy and design largely locked. ✅
- Case study pages — not started yet. The homepage is the design template.

## Running it
It's a static site. Just open `index.html` in a browser, or serve the folder:
```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```
Fonts load from Google Fonts; nothing to install.

## Deploying
Drop the folder on any static host (Netlify, Vercel, GitHub Pages, Cloudflare Pages). No build command, no framework.

---

## Design system (already in `:root` of index.html)

**Colors**
- `--bg: #F7F6F3` warm off-white
- `--ink: #1A1A1A` near-black text
- `--ink-mid: #5A5753` secondary text
- `--ink-light: #9C9890` tertiary/labels
- `--rule: #E2E0DC` hairline dividers
- `--accent: #2251CC` accessible cobalt blue (passes WCAG AA on bg)

**Type**
- Display: DM Serif Display (used with restraint; italic = the "signature" treatment)
- Body/UI: Inter

**Signature move:** one word per section set in italic serif accent blue (e.g. *actually*, *interrogate*, *tangled*). Used sparingly. Don't let it spread or it stops meaning anything.

**Layout:** generous whitespace, 1080px max width, hairline rules instead of cards/shadows, editorial feel.

---

## Voice & copy rules (IMPORTANT — this is the hard-won part)

Sally's voice: **dry, a little sarcastic, heart of gold.** Likes puzzles and complicated problems. Casual is fine in small doses; keep it classy. No swearing beyond mild.

She communicates concise, direct, constraint-driven. Expects copy to be defensible. Asks for things to be *shortened*, not embellished.

**Anti-patterns to NEVER reintroduce (these are AI tells):**
- The "isn't X, it's Y" / "not because X, but because Y" reversal construction. Overused. Avoid.
- Em-dashes as a default clause-joiner. Currently only ONE in the file (the page `<title>`). Keep it that way — use periods, colons, parentheses instead.
- Thesaurus runs: don't stack synonyms (had "pressure-test / stress-test / interrogate" all at once — now just "interrogate").
- Filler like "with intention," "seamless," "passionate," "leverage," "elevate."
- Generic agency CTAs ("Let's talk," "Got a project?").

**Keep:** plain specific sentences, the occasional deadpan beat ("Those are the options."), real numbers and concrete examples (4 chars vs 40, 6-digit dollar amounts).

---

## The story the site tells
- ~10 years at Crafted (15-person agency). Loyalty framed as a *character trait*, not a Crafted ad. Stat reads "One firm, by choice."
- Started as a developer (code bootcamp era), grew into design. Designer-developer hybrid is a real differentiator, amplified by AI.
- Sole designer = the entire design function. AI workflow is how one person produces team-scale output.
- Niche: dense, enterprise B2B. Dashboards, admin tools, native apps, design systems.

## Process section (her actual workflow — don't generic-ify)
1. **Interrogate the PRD** — hands the real PRD to Claude, checks her read, finds gaps before designing.
2. **Generate real content** — no lorem ipsum; realistic variance to break layouts early.
3. **High-fidelity directly** — no wireframes; hi-fi is the fast iteration now.
4. **Own it through handoff** — tokens, component docs, React prototypes.

Toolkit (AI tools highlighted in blue pills): Figma, Figma MCP, Claude, Claude Code, Cursor + React, Design Tokens, Design Systems.

---

## Case study to build first: Regional Grid Operator — Native App
This is MISO, but **must be referred to vaguely** (no "MISO" name) for confidentiality. "Regional grid operator" is the framing.

Public, citable stats (no NDA issues — these are public-record facts about the operator, not Crafted's work):
- Serves ~42 million people across 15 US states + Manitoba
- ~186,000 MW market capacity, ~72,000 miles of transmission lines
- Real-time data updated every 5 seconds (303,800 data points in the public system)
- Wholesale market settles ~$2 billion/month

Screenshots for this case study live in the uploads (mobile real-time displays: generation fuel mix, real-time LMP, schedule interface, ACE charts, ancillary market).

**Stats Sally still needs to gather internally** for other potential case studies: # of shops on NexsyisNow, USA Football registered orgs/users, app store ratings, design-system component counts.

## Open copy decisions (Sally to confirm)
- Contact headline: "Got something *tangled*? That's my favorite kind." — possibly too cute? drier alt: "That's the fun part."
- Footer: "Yes, I built this one too." — keep or simplify?

---

## Picking this up in Claude Code
1. Download this folder to your machine.
2. `cd` into it and open it with Claude Code.
3. Point Claude Code at this README first — it carries the voice rules, design tokens, and the MISO confidentiality constraint.
4. Suggested next task: build `grid-operator.html` using `index.html` as the visual template.
