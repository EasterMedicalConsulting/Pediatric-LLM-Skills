# AF Peds Resident — LLM Skill Kit

A collection of prompt templates ("skills") to help Air Force pediatric residents leverage any large language model (LLM) to produce high-quality clinical and administrative documents faster. These skills work with any LLM — Claude, ChatGPT, Gemini, Copilot, etc. — and require no special software or plugins.

---

## What's in this kit

| Skill | Folder | What it produces |
|---|---|---|
| **OPB Template** | `opb-template/` | AF-style performance bullets for Officer Performance Brief / OPR |
| **MFR Template** | `mfr-template/` | Tongue & Quill–compliant Memorandum for Record |
| **Patient Letters** | `patient-letters/` | Medical necessity, school medication auth, EFMP letters, accommodations |
| **Dot Phrases** | `dot-phrases/` | Cerner My AutoText dot phrases — well-child, acute visits, EFMP |
| **Disciplinary Action** | `disciplinary-action/` | RIC, LOC, and LOR — AFI 36-2907 compliant administrative discipline documents |

---

## How to use any skill

1. Open the `SKILL.md` file in the skill folder you need.
2. Copy the **entire prompt block** (clearly marked in each file between `===START===` and `===END===`).
3. Open any LLM chat interface and paste it in.
4. The LLM will ask you questions one at a time — answer them.
5. Copy the finished output directly into your document, letter, or note.

That's it. No account setup, no tools, no integrations required.

---

## LLM options

Any modern LLM works. Pick whatever is accessible on your network:

- **Claude** (claude.ai) — strong at structured documents and following format rules precisely
- **ChatGPT** (chatgpt.com) — widely accessible; use GPT-4o for best results
- **Gemini** (gemini.google.com) — solid for document drafting; integrates with Google Workspace
- **Microsoft Copilot** — available on many .mil networks via M365

If you're at an installation with restricted internet, check with your local communications squadron about which AI tools are approved for use.

---

## A word on patient data

These skills generate drafts from information you provide. If you are working on a system or platform that is **not** approved for PHI, use placeholder values during any practice or testing run (e.g., "Patient A", "DOB: XX/XX/XXXX", "[PATIENT NAME]"). Always verify clinical accuracy before signing or sending any output.

---

## A word on disciplinary action documents

The RIC / LOC / LOR skill produces drafts only. **Always have your Staff Judge Advocate (SJA) review any Letter of Reprimand before it is signed and issued.** LOCs should be reviewed by your supervisor chain and commander. These documents have real career consequences for the member — accuracy and legal defensibility matter.

---

## Tips for better output

- **Be specific.** The more concrete detail you give (numbers, dates, outcomes), the better the output.
- **One question at a time.** The prompts ask the LLM to go question-by-question — let it. Don't dump everything at once.
- **Iterate.** After output is generated, tell the LLM "make bullet 3 stronger" or "the letter tone should be more formal." It will revise.
- **Save your prompt inputs.** If you build a dot phrase or letter you like, save the answers you gave as a personal template so next time is even faster.

---

## Folder structure

```
af-peds-llm-skills/
├── README.md                      ← You are here
├── opb-template/
│   └── SKILL.md
├── mfr-template/
│   └── SKILL.md
├── patient-letters/
│   └── SKILL.md
├── dot-phrases/
│   └── SKILL.md
└── disciplinary-action/
    └── SKILL.md
```

---

*Built for AF pediatric residents transitioning to their first duty assignments. Skills are plain `.md` files — open with any text editor, Notepad, VS Code, or a Markdown viewer.*
