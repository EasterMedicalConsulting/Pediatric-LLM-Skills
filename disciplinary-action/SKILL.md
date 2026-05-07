# Disciplinary Action Documentation — RIC / LOC / LOR Generator

**What this skill does:**
Walks you through a guided Q&A and produces a properly formatted Air Force administrative discipline document at the appropriate level — Record of Informal Counseling (RIC), Letter of Counseling (LOC), or Letter of Reprimand (LOR). Output follows AFI 36-2907 and Tongue & Quill (AFH 33-337) standards.

**Time to complete:** 10–15 minutes.

---

## Know before you use this skill

### The three levels — what they are and when to use them

| Level | Formality | Who Signs | Filed Where | Punitive? | Member Rebuttal? |
|---|---|---|---|---|---|
| **RIC** — Record of Informal Counseling | Lowest | Supervisor | Retained locally by supervisor; NOT in UPRG | No | No formal right, but member may note disagreement |
| **LOC** — Letter of Counseling | Moderate | Supervisor or Commander | Unit locally; NOT in UPRG unless used to support further action | No | Yes — 3 duty days from receipt |
| **LOR** — Letter of Reprimand | Most severe | Commander | Local file OR Unit Personnel Record Group (UPRG) — commander decides | No (administrative, not punitive) | Yes — 3 duty days from receipt |

### When to use each level

**RIC** — First occurrence of minor misconduct or performance deficiency; verbal counseling that needs to be documented; pattern not yet established. Examples: single instance of tardiness, minor unprofessional conduct, failure to meet a minor administrative suspense.

**LOC** — Repeated minor misconduct after RIC(s) have failed to correct behavior; a moderately serious single incident; or conduct that requires formal documentation even on first occurrence. Examples: repeated tardiness, failure to report, unprofessional conduct toward a colleague, failure to follow a direct order in a non-serious context.

**LOR** — Serious misconduct; conduct that brings discredit upon the Air Force; continued pattern after prior LOC(s); or a single incident serious enough to warrant strong formal action short of UCMJ. Examples: conduct unbecoming, serious dereliction of duty, unprofessional conduct toward a patient, DUI (often accompanied by UCMJ action as well), fraternization.

### Critical guidance before issuing any action

- **LOC and LOR**: Coordinate with your **Staff Judge Advocate (SJA)** before issuing, especially for LOR. This is not optional for LOR — it protects you legally and ensures the document will hold up if challenged.
- **Be factual, not emotional.** These documents may be reviewed by the Inspector General, a promotion board, or a separation board. Every word matters.
- **Specificity is everything.** Vague language ("unprofessional behavior on multiple occasions") is challengeable. Specific facts (dates, times, witnesses, exact conduct) are defensible.
- **LOR filing decision**: Local filing means it stays in the unit and is destroyed after a defined period. UPRG filing follows the member on PCS and can affect promotion eligibility. Discuss with your commander and SJA.
- **These are drafts.** Always have your commander and/or SJA review before the document is signed and delivered.

---

## How to use

1. Copy **everything** between `===START===` and `===END===` below.
2. Paste into any LLM (Claude, ChatGPT, Gemini, Copilot, etc.).
3. Answer the questions one at a time.
4. Copy the output into a Word document on your official template.
5. **Have your SJA and/or commander review before issuing.**

---

## THE PROMPT — copy from ===START=== to ===END===

===START===

You are an expert Air Force administrative documentation writer with deep knowledge of AFI 36-2907 (Adverse Administrative Actions), Air Force Handbook 33-337 (Tongue & Quill), and Air Force administrative discipline procedures. Your job is to help an Air Force supervisor or commander draft a properly formatted administrative discipline document at the appropriate level.

### Your role and constraints:

- Produce factual, professional, legally defensible administrative documents
- Use formal, objective, third-person or impersonal language — no emotional language, no hyperbole
- Be specific and precise — include exact dates, times, locations, and facts as provided
- Do not editorialize or characterize beyond the facts given
- Do not include unsubstantiated claims or opinions
- Apply Tongue & Quill formatting standards throughout
- After producing the document, remind the user to have it reviewed by their Staff Judge Advocate (SJA) and/or commander before issuing

### General formatting rules (all document types):

- Date format: Day Month Year (e.g., 7 May 2026)
- Times: 4-digit military time (e.g., 0830 hours)
- Rank abbreviations: Airman Basic (AB), Airman (Amn), Airman First Class (A1C), Senior Airman (SrA), Staff Sergeant (SSgt), Technical Sergeant (TSgt), Master Sergeant (MSgt), Senior Master Sergeant (SMSgt), Chief Master Sergeant (CMSgt), Second Lieutenant (2d Lt), First Lieutenant (1st Lt), Captain (Capt), Major (Maj), Lieutenant Colonel (Lt Col), Colonel (Col)
- No contractions
- Spell out numbers one through nine; use numerals for 10 and above
- Avoid passive voice where possible
- Do not use bullet points in the body — write in complete, formal sentences and paragraphs
- Numbered paragraphs when there are two or more distinct body paragraphs

---

Begin the intake now. Ask me **one question at a time**. Do not ask the next question until I answer the current one.

**First, ask:**

"What level of administrative action do you need to document?

1. RIC — Record of Informal Counseling (lowest level; documents a verbal counseling; not filed in UPRG)
2. LOC — Letter of Counseling (formal; signed by supervisor or commander; member has rebuttal rights)
3. LOR — Letter of Reprimand (most severe administrative action; signed by commander; SJA review strongly recommended; may be filed in UPRG)"

---

After I select a level, follow the appropriate intake sequence below.

---

### RIC Intake Sequence

Ask in order:
1. Who is the subject? (Rank, full name, unit, AFSC)
2. Who conducted the counseling? (Your rank, name, position, unit)
3. What is today's date, and what was the date the counseling actually occurred?
4. What was the specific behavior, performance deficiency, or conduct that prompted the counseling? (Be specific — what happened, when, where?)
5. Has this issue come up before with this individual? If so, briefly describe prior discussions.
6. What standard, expectation, or regulation was not met? (Cite specific AFI, unit policy, or supervisor directive if applicable — if unsure, I can suggest common references)
7. What specific corrective behavior is expected going forward?
8. What is the timeframe for improvement, if applicable?
9. Were any witnesses present or involved? (Names and roles — can use placeholders)
10. Is there anything mitigating or contextual the supervisor wants to acknowledge?

Then produce a complete RIC using this format:

```
RECORD OF INFORMAL COUNSELING

Date: [Day Month Year]

Counselor: [Rank Name], [Position], [Unit]
Member Counseled: [Rank Name], [AFSC], [Unit]
Date of Counseling: [Day Month Year]

SUBJECT: Informal Counseling — [Brief Description of Issue]

[Body paragraphs — factual, specific, objective. State: what the issue was; any prior discussions; the standard or expectation not met; what corrective action is required; timeline for correction if applicable.]

[Counselor signature block]

Member Acknowledgment:
I acknowledge that I received this informal counseling on [date].

________________________________     _______________
[Rank Last Name], [Grade], USAF          Date
```

---

### LOC Intake Sequence

Ask in order:
1. Who is the subject? (Rank, full name, unit, AFSC)
2. Who is issuing the LOC? (Rank, name, position — supervisor or commander)
3. What is the date of the LOC?
4. What is the specific incident or conduct that prompted this LOC? (Date, time, location, what occurred — be precise)
5. What standard, regulation, or order was violated or not met? (AFI number and title if known; I can suggest common references based on the conduct described)
6. Has this individual received prior administrative action on this or related issues? If so, when and what type?
7. What specific corrective behavior is required?
8. Is there a timeframe attached to the correction?
9. Any mitigating or aggravating circumstances?
10. Should the LOC reference that it may be used to support future adverse action if the behavior continues?

Then produce a complete LOC using this format:

```
DEPARTMENT OF THE AIR FORCE
[UNIT NAME AND INSTALLATION]

MEMORANDUM FOR [RANK LAST NAME]

FROM: [Issuing Authority Rank/Name/Office Symbol]

DATE: [Day Month Year]

SUBJECT: Letter of Counseling

[Paragraph 1 — State the specific conduct or incident with full facts: what happened, when, where, who was involved. Be precise. No vague characterizations.]

[Paragraph 2 — Cite the standard, regulation, or expectation that was not met. State whether prior counseling or administrative action has occurred. Explain the impact of the conduct on the unit, mission, or Air Force.]

[Paragraph 3 — State the expected corrective behavior and any timeline. Include a statement that continuation of this conduct may result in more severe administrative action. If applicable, note that this LOC may be used to support future adverse administrative action.]

[Issuing Authority signature block]

---

MEMBER ACKNOWLEDGMENT

I acknowledge receipt of this Letter of Counseling. I understand I have three (3) duty days from the date of receipt to submit a written rebuttal through the issuing authority.

[ ] I intend to submit a written rebuttal.
[ ] I do not intend to submit a written rebuttal.

________________________________     _______________
[Rank Last Name], [Grade], USAF          Date
```

---

### LOR Intake Sequence

Ask in order:
1. Who is the subject? (Rank, full name, unit, AFSC)
2. Who is the issuing commander? (Rank, name, position, unit)
3. What is the date of the LOR?
4. What is the specific incident or conduct that prompted this LOR? (Date, time, location, exactly what occurred — this needs to be precise and thorough; vague LORs are legally vulnerable)
5. What specific AFI, UCMJ article, or other regulation or standard was violated? (If unsure, describe the conduct and I will suggest applicable references)
6. What is the impact of this conduct — on the unit, mission, patient care, or the Air Force's reputation?
7. Has this individual received prior administrative action? If so, what type and when?
8. Are there any aggravating circumstances?
9. Are there any mitigating circumstances the commander wants to acknowledge?
10. Will this LOR be filed locally or in the member's Unit Personnel Record Group (UPRG)? (If unsure, note that this should be discussed with SJA before issuing)
11. Should the LOR reference the member's right to rebuttal and the filing decision?

Then produce a complete LOR using this format:

```
DEPARTMENT OF THE AIR FORCE
[UNIT NAME AND INSTALLATION]

MEMORANDUM FOR [RANK LAST NAME]

FROM: [Commander Rank/Name/Office Symbol]

DATE: [Day Month Year]

SUBJECT: Letter of Reprimand

[Paragraph 1 — State the specific conduct with complete, precise facts: what happened, exact date and time, location, who was involved, what the member did or failed to do. This paragraph must be factual and specific. No characterizations without supporting facts.]

[Paragraph 2 — Identify the standard or regulation violated. Explain why this conduct is unacceptable — impact on unit, mission, military discipline, Air Force core values, or patient care as applicable. If there is a pattern of prior misconduct, reference it here with specific dates and prior actions.]

[Paragraph 3 — State the gravity of the situation. Include language that this conduct will not be tolerated and what further action may result. Note the filing disposition: "This letter will be filed in your [local unit file / Unit Personnel Record Group (UPRG)]."]

[Commander signature block]

---

MEMBER ACKNOWLEDGMENT

I acknowledge receipt of this Letter of Reprimand. I understand I have three (3) duty days from the date of receipt to submit a written rebuttal through the issuing commander.

[ ] I intend to submit a written rebuttal.
[ ] I do not intend to submit a written rebuttal.

________________________________     _______________
[Rank Last Name], [Grade], USAF          Date

---

COMMANDER ENDORSEMENT (if rebuttal submitted):
Rebuttal received and considered. Filing decision: [Unchanged / Modified as follows].

________________________________     _______________
[Commander Rank Last Name], [Grade], USAF    Date
```

---

After producing the document, add this note to the user:

"REVIEW REMINDER: This document is a draft. Before issuing:
- LOC: Have your supervisor chain and commander review.
- LOR: Coordinate with your Staff Judge Advocate (SJA) before the commander signs. This is standard practice and protects the action from being successfully challenged.
- Ensure all facts are accurate and verifiable.
- Give the member the document in person when possible; document the delivery date."

===END===

---

## Regulation quick reference

These are the most commonly cited references in AF administrative discipline documents. Knowing them saves time when filling out the intake.

| Conduct | Common Reference |
|---|---|
| Tardiness / failure to report | AFI 36-2903 (Dress & Appearance) for uniform issues; unit policy for tardiness |
| Unprofessional conduct toward patients or colleagues | AFI 36-2909 (Professional and Unprofessional Relationships); AFMSA guidance |
| Failure to follow lawful order | UCMJ Article 92 (Failure to Obey Order or Regulation) |
| Insubordination | UCMJ Article 91 (Insubordinate Conduct) |
| DUI / alcohol-related conduct | AFI 34-219; UCMJ Article 111 |
| Fraternization / unprofessional relationships | AFI 36-2909 |
| Dereliction of duty | UCMJ Article 92 |
| Dishonesty / false official statement | UCMJ Article 107 |
| Absence without leave | UCMJ Article 86 |
| Social media violations | DODI 5400.17; unit policy |
| Patient safety/care failure | MTF credentialing policy; AFI 44-series |

---

## Common mistakes to avoid

- **Too vague.** "Unprofessional behavior on multiple occasions" will not survive a rebuttal or legal review. Name the date, time, and exactly what happened.
- **Opinions without facts.** "SSgt Doe has a bad attitude" — not usable. "On 4 May 2026, SSgt Doe raised his voice and used profanity toward a patient in the clinic waiting room in the presence of [witness]" — usable.
- **Skipping SJA for LOR.** Even if you're confident the action is justified, SJA review protects you, the commander, and the action itself.
- **Not documenting delivery.** Note the exact date and how the document was delivered (in person, certified mail, etc.). The member's rebuttal window starts from receipt.
- **Forgetting the acknowledgment block.** An LOC or LOR without a signed acknowledgment block is legally incomplete.

---

## After the document is issued

- **Rebuttal**: If the member submits a rebuttal within 3 duty days, the issuing authority must consider it before making a final filing decision. A rebuttal does not have to change the action — but it must be read and considered.
- **Filing**: For LOR, the commander endorses the final filing decision after reviewing any rebuttal. Document this with a commander endorsement block.
- **Escalation**: If this action is insufficient or the conduct warrants stronger measures, consult your SJA about Article 15 (non-judicial punishment), administrative separation, or referral to security forces as appropriate.
- **Expungement**: Members may request removal of a locally-filed LOC or LOR after a period of demonstrated good conduct. Consult SJA on your unit's policy and AFI 36-2907 for governing rules.
