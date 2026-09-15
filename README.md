<div align="center">

# 伟大的你 · Great You

**English** | [简体中文](./README.zh-CN.md)

</div>

> Turn a fleeting reflection into a philosophical monograph — with thought tracing, a way out, and a personal action pledge.

A **cross-platform Agent Skill** — a pure `SKILL.md` workflow that runs on WorkBuddy, Claude Code, or any AI agent that can load skill / prompt files. When you jot down a stray thought about life, work, or meaning, this skill doesn't rush to typesetting. It first sits you down for a conversation with the greatest minds who wrestled with the same questions — and only after the discussion settles does it produce a single-file HTML monograph.

📖 **[See the full example *Seeing What Matters*](./example/monograph.html)** (a monograph on overcoming snap judgments by appearance — open in browser)

---

## ✨ Core Principles

**Discuss first, produce last.** Typesetting is the final step of the pipeline, never the first.

**Great minds and great works over online opinions.** Discussion draws only on classic texts in the model's knowledge; web opinions are never searched. WebSearch is allowed for one thing only — verifying the exact wording and source of quotations.

**Zero fabricated quotes.** Every quotation must be checked against a published Chinese translation; if no reliable source can be found, it stays unquoted.

## 🔄 Workflow (Six Steps, in Order)

| Step | Name | What happens |
|---|---|---|
| 0 | **Discuss First** | Explore the reflection through classic writers and works in a back-and-forth dialogue — no output, no layout, until the direction is settled and user-approved |
| 1 | **Life Notes** | Distill the thought into three progressive notes (a single sentence becomes "insight → predicament → exit"), closing with a punchline |
| 2 | **Philosophical Echo** | Anchor each note to 1–2 writers with original quotations; WebSearch verifies wording and sources only |
| 3 | **The Way Out** | A diagnosis (two forces closing in) + three moves (Subtraction / Conversion / Second Space) + Nietzsche's eternal-return calibrator |
| 4 | **My Pledge** | Three concrete, this-week-startable actions, each with how-to, pitfalls, and a checkable box |
| 5 | **Typesetting** | Only after everything is finalized and user-approved: assemble a single-file HTML monograph |

## 📖 Monograph Chapters

```
〇  Roundtable        Great minds speak across disciplines (philosophy / psychology / sociology / literature)
i   Life Notes        Three progressive notes + a punchline
ii  Echo              Writer quote cards (life dates + work + source + commentary) + a synthesis
iii The Way Out       Diagnosis + three moves + calibrator
iv  My Pledge         Three checkable weekly actions + signed seal ("记")
v   Figures & Reading Person guide (consistency check: zero missing, zero extra)
```

## 💬 Example Session

```
You:   Work feels like spinning in place — busy all day, unsure what got done.
       Make me a knowledge card to record this state.

AI:    (Step 0) This echoes Marx's "alienated labor" and Schopenhauer's "boredom"…
       (a few rounds of discussion until you approve the direction)

AI:    Content settled. (Steps 1–4) Three notes → verify quotes from the
       1844 Manuscripts → three moves → three weekly actions.

AI:    (Step 5) Typesetting done → /workspace/monograph.html ✅
```

Typical triggers: *"make me a knowledge card for this"* / *"organize this reflection"* / *"thought tracing"* / *"has any writer said this?"* / *"how do I break out of this state?"*

## 📦 Installation

**WorkBuddy** — clone into a skills directory:

```bash
# User-level (available in all projects)
git clone https://github.com/Dassin/great-you.git ~/.workbuddy/skills/great-you

# Or project-level
git clone https://github.com/Dassin/great-you.git .workbuddy/skills/great-you
```

**Claude Code** — drop it into your skills folder:

```bash
git clone https://github.com/Dassin/great-you.git ~/.claude/skills/great-you
```

**Any other agent** — the whole skill is one `SKILL.md` plus one HTML template: paste the workflow into your agent's system prompt / custom instructions / project rules (ChatGPT Projects, Claude Projects, etc.) and it just works. Restart your agent session and it's live.

## 🎨 Visual System (Series Consistency)

- **Background**: dark textured gradient `linear-gradient(160deg,#0f1419,#1a1625,#14110d)` with ochre-gold / violet-red glows
- **Cards**: beige paper `#f7f2e8 → #efe8d6`, 12px radius, deep shadow + paper texture
- **Accents**: ochre-gold `#c9a961` (titles / numerals / dividers), vermilion `#b8683a` (diagnosis / pitfalls / seal)
- **Fonts**: Noto Serif SC (Chinese serif) + Cormorant Garamond (Roman-numeral chapter numerals)
- **Quote blocks**: 3px ochre-gold left rule + serif body + small-print source
- **Signature**: date + vermilion round seal ("记", rotated −8°)
- **Contrast rule**: light text only on the dark body; all text inside beige cards must be dark

Full skeleton in [`assets/monograph-template.html`](./assets/monograph-template.html) — copy the structure, replace the placeholders.

## 📁 Repository Layout

```
great-you/
├── SKILL.md                        # skill definition (full workflow)
├── README.md                       # this file (English)
├── README.zh-CN.md                 # Chinese readme
├── assets/
│   └── monograph-template.html     # monograph skeleton (placeholder version)
└── example/
    └── monograph.html              # real output: "Seeing What Matters"
```

## ✅ Quality Guarantees

1. **Figure-consistency check**: before finalization, the set of figures appearing in the text must exactly match the "Figures & Readings" chapter — zero missing, zero extra, every entry tagged with *nationality · era · life dates*
2. **Quote verification**: all quoted text is checked against published Chinese translations (Records of the Grand Historian, Zhuangzi, Liezi, Kant's Anthropology, The Little Prince, The Society of the Spectacle, The Consumer Society, the 1844 Manuscripts, The Gay Science, etc.), cited down to the translator
3. **Discuss before layout**: never typeset before the user approves the content

## License

MIT © 2026 FengSun
