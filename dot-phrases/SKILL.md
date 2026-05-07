# Dot Phrases — Cerner My AutoText Builder for Pediatric Providers

**What this skill does:**
Generates ready-to-use dot phrase text blocks for Cerner's **My AutoText** feature (used in MHS Genesis / PowerChart). You answer a few questions about your practice patterns and the LLM produces customized dot phrase text you can copy directly into Cerner.

**Time to complete:** 5–15 minutes per phrase, depending on complexity.

---

## What is a Cerner My AutoText dot phrase?

In Cerner PowerChart (MHS Genesis), My AutoText phrases are saved text blocks you can insert into any note by typing a short keyword starting with a period. For example:

- You type `.wc2mo` → it expands to your full 2-month well-child visit template
- You type `.omplan` → it expands to your otitis media treatment plan
- You type `.efmpsupport` → it expands to your EFMP documentation block

**How to add a phrase to Cerner:**
1. In PowerChart, go to **Tools → My AutoText**
2. Click **New**
3. Enter your **abbreviation** (the keyword — no period needed here; Cerner adds it)
4. Enter the **full text** of the phrase
5. Save

The LLM output from this skill gives you both the recommended abbreviation and the full text to paste into the "full text" field.

---

## Dot phrase categories included

| # | Category | What it covers |
|---|---|---|
| 1 | **Well-Child Visits** | Age-specific physical exam, anticipatory guidance, screening documentation |
| 2 | **Acute Sick Visits** | Common peds diagnoses — otitis media, URI, pharyngitis, croup, bronchiolitis, GI illness, fever, UTI, rash |
| 3 | **EFMP / Administrative** | EFMP enrollment documentation, PCS support language, special needs care summaries |
| 4 | **Custom / Other** | Any phrase you can describe — the LLM will build it |

---

## How to use

1. Copy **everything** between `===START===` and `===END===` below.
2. Paste into any LLM (Claude, ChatGPT, Gemini, Copilot, etc.).
3. Tell the LLM which category and specific type of phrase you need.
4. Answer the customization questions.
5. Copy the output directly into Cerner My AutoText.

### Naming convention recommendations

Keep abbreviations short (5–10 characters), memorable, and organized:
- Prefix by type: `wc` = well child, `ac` = acute, `efmp` = EFMP
- Then a descriptor: `wc2mo`, `wcnb`, `acom`, `acuri`, `efmpenroll`
- Avoid generic names — you'll accumulate many phrases over time

---

## THE PROMPT — copy from ===START=== to ===END===

===START===

You are an expert pediatric physician clinical documentation assistant helping an Air Force pediatrician create Cerner My AutoText dot phrases for use in MHS Genesis / PowerChart.

### Output format rules you must always follow:

1. **Provide a recommended abbreviation** — short (5–10 chars), no spaces, lowercase, memorable. Prefix with category: `wc` (well child), `ac` (acute), `efmp` (EFMP/admin), or other logical prefix.
2. **Provide the full dot phrase text** in a clean code block — ready to copy and paste into Cerner. No markdown formatting in the output text (no bold, no headers) — Cerner is a plain text field.
3. Use **[BRACKETS]** for fields the provider needs to fill in at the time of the note — e.g., `[WEIGHT]`, `[PARENT NAME]`, `[AGE]`, `[CHIEF COMPLAINT]`.
4. Keep language **clinically appropriate and concise** — this is documentation, not an essay.
5. Structure the text with **natural line breaks** so it reads cleanly when pasted into a note.
6. For well-child visits, include **age-appropriate anticipatory guidance topics** based on Bright Futures guidelines (4th edition).
7. For acute visits, include **evidence-based treatment plans** using current AAP guidelines where applicable.

---

Begin now. Ask me the following questions **one at a time**. Do not ask the next question until I answer the current one.

**First, ask:**

"What type of dot phrase do you need? Choose a number or describe what you want:

1. Well-Child Visit — specify age (e.g., 2-month, 9-month, 2-year, 5-year, adolescent)
2. Acute Sick Visit — specify condition (e.g., otitis media, croup, URI, pharyngitis, bronchiolitis, UTI, fever, GI illness, rash, head injury)
3. EFMP / Administrative — specify type (enrollment support note, PCS letter documentation, annual update note, special needs care summary)
4. Custom — describe what you need and I'll build it"

---

After I select a type, follow the appropriate intake sequence below.

---

### Category 1 — Well-Child Visit Dot Phrase

Ask in order:
1. What age visit is this for? (e.g., newborn, 2 week, 1 month, 2 month, 4 month, 6 month, 9 month, 12 month, 15 month, 18 month, 24 month, 30 month, 3 year, 4 year, 5 year, 6–10 year, 11–17 year / adolescent)
2. What sections do you want in the template? (Choose all that apply: chief complaint line, interval history, nutrition/feeding, development/milestones, physical exam, screening results, vaccines administered, anticipatory guidance topics, plan/return to clinic)
3. Are there any clinic-specific phrases, abbreviations, or standing orders you want included? (e.g., your clinic's standard fluoride recommendation, specific vaccine schedule notes, lead screening at 12 and 24 months)
4. Do you want the developmental milestone section to include specific milestones to check off, or just a free-text field?
5. For anticipatory guidance — do you want the full Bright Futures list for that age, a curated short list, or just [AG DISCUSSED] placeholders?

Then generate:
- **Recommended abbreviation**
- **Full dot phrase text** — complete, ready to paste into Cerner

---

### Category 2 — Acute Sick Visit Dot Phrase

Ask in order:
1. What condition or chief complaint is this phrase for?
2. What sections do you want? (Choose all that apply: chief complaint, HPI, pertinent positives/negatives, physical exam findings, assessment/diagnosis with ICD-10 code, treatment plan, return precautions, follow-up instructions)
3. Do you want the assessment to include the ICD-10 code in-line, or just the diagnosis name?
4. For the treatment plan — do you want specific medication options with dosing guidance as a template, or just `[TREATMENT PLAN]` placeholders?
5. Do you want return precautions listed as a standardized block, or customized for this specific diagnosis?
6. Are there any clinic-specific protocols (e.g., your MTF's strep testing policy, specific antibiotic formulary) I should build into the template?

Then generate:
- **Recommended abbreviation**
- **Full dot phrase text** — complete, ready to paste into Cerner

After generating, offer to create a companion phrase — e.g., if I build an otitis media acute visit note, offer to also build `.omreturn` for the return visit template.

---

### Category 3 — EFMP / Administrative Dot Phrase

Ask in order:
1. What type of EFMP documentation do you need? (Initial enrollment support note, annual update, PCS transition note, special needs care summary, developmental delay documentation, therapy services justification)
2. What diagnoses or conditions are typically documented in this note type?
3. What services should the template reference? (e.g., speech therapy, OT, PT, behavioral health, subspecialty care, educational support, durable medical equipment)
4. Should the template include a section for documenting service frequency and location requirements (important for PCS planning)?
5. Should the note include a standard closing statement directing families to their EFMP coordinator?

Then generate:
- **Recommended abbreviation**
- **Full dot phrase text** — complete, ready to paste into Cerner

---

### Category 4 — Custom Dot Phrase

Ask in order:
1. Describe what this phrase is for and what it should say.
2. What sections or components should it have?
3. Are there specific clinical statements, regulatory language, or standard phrases I should include?
4. What should be left as fill-in fields `[IN BRACKETS]` versus pre-populated text?
5. Should there be any conditional branching (e.g., "if breastfeeding: X / if formula: Y") or will this be a single linear template?

Then generate:
- **Recommended abbreviation**
- **Full dot phrase text** — complete, ready to paste into Cerner

===END===

---

## Example output — 2-Month Well-Child Visit

**Recommended abbreviation:** `wc2mo`

**Full dot phrase text (paste into Cerner My AutoText):**

```
2-MONTH WELL CHILD VISIT

CC: [PATIENT NAME] is a 2-month-old presenting for well-child care. Parent/guardian: [PARENT NAME].

INTERVAL HISTORY:
No significant illnesses since last visit. No ER visits or hospitalizations.
Feeding: [Breastfeeding / Formula — type and amount per feed / day]. No feeding concerns reported.
Sleep: [SLEEP PATTERN]. Placed supine for all sleep. Own sleep surface.
Voiding/stooling: [NORMAL / DESCRIBE].
Social history: Lives with [DESCRIBE HOUSEHOLD]. No tobacco smoke exposure.

DEVELOPMENT:
Social smile: [present / not yet]
Tracks objects to midline: [yes / no]
Coos: [yes / no]
Lifts head when prone: [yes / no]
Parent concern: [none / DESCRIBE]

PHYSICAL EXAM:
General: Well-appearing, alert, non-toxic, in no acute distress.
HEENT: Normocephalic, atraumatic. Anterior fontanelle open and flat. Eyes: PERRL, no discharge. Ears: TMs clear bilaterally. Oropharynx: clear, moist mucous membranes. Neck: supple, no lymphadenopathy.
Resp: Clear to auscultation bilaterally. No work of breathing.
CV: Regular rate and rhythm. No murmur. Femoral pulses 2+ bilaterally.
Abdomen: Soft, non-distended, non-tender. No hepatosplenomegaly. Umbilical stump [healed / describe].
GU: [Normal male / Normal female / describe]. Testes [descended bilaterally / describe].
MSK: Full range of motion all extremities. Hips: Ortolani/Barlow negative. No deformity.
Skin: No rash, no lesions. [Birthmarks: describe or none].
Neuro: Tone appropriate for age. Moro, grasp, and rooting reflexes present.

SCREENING:
Developmental screening: [M-CHAT not applicable at this age — Bright Futures developmental surveillance completed].
Autism: [N/A at this age].
Lead: [N/A — will screen at 12 months].
Anemia: [N/A — will screen at 12 months].
Hearing: [Newborn screen passed per parent report / documented in record].
Vision: [Red reflex symmetric bilaterally].

IMMUNIZATIONS TODAY:
[DTaP / IPV / Hib / PCV15 / Hep B (if dose 2 due) / RV — per current ACIP schedule]
VIS provided and reviewed. Parent questions answered. Benefits and risks discussed.

ANTICIPATORY GUIDANCE DISCUSSED:
- Safe sleep: supine, firm flat surface, own sleep space, no soft bedding
- Feeding: on demand breastfeeding or [X] oz formula q[X] hours; no water, juice, or solids
- Car safety: rear-facing infant seat, back seat, never leave in hot car
- Tummy time: minimum 30 minutes per day when awake and supervised
- No screen time
- Shaken baby syndrome / never shake prevention counseling provided
- Developmental stimulation: talking, reading, skin-to-skin
- Handwashing and illness prevention
- Smoke and environmental exposure avoidance
- Vitamin D supplementation [400 IU daily if breastfed or <32oz formula/day]

PLAN:
1. Continue current feeding plan.
2. [ADDITIONAL PLAN ITEMS AS APPLICABLE]
3. Immunizations administered as above.
4. Return to clinic: 4-month well-child visit.
5. Call or return for: fever >100.4F, inconsolable crying, poor feeding, vaccine reaction concerns.

Provider: [YOUR NAME, DEGREE]
Date: [DATE]
```

---

## Example output — Otitis Media Acute Visit

**Recommended abbreviation:** `acom`

**Full dot phrase text:**

```
ACUTE VISIT — OTITIS MEDIA

CC: [PATIENT NAME] is a [AGE]-year-old presenting with [ear pain / fever / irritability / pulling at ears / hearing changes] x [DURATION].

HPI:
Onset [ACUTE / GRADUAL]. Symptoms include [ear pain — right / left / bilateral], [fever — max temp: TEMP], [irritability], [decreased appetite], [URI symptoms — runny nose, congestion x DAYS]. No prior ear infections in the last [X] months / [FIRST EPISODE]. [Prior ear tubes — yes / no]. No vomiting, no neck stiffness, no rash.

PHYSICAL EXAM:
General: [Well-appearing / Mildly ill-appearing], non-toxic.
HEENT: TM — [Right: erythematous, bulging, opaque, decreased mobility / normal]. [Left: erythematous, bulging, opaque, decreased mobility / normal]. No perforation. No discharge. No post-auricular erythema or tenderness. Oropharynx: [clear / erythematous, no exudate]. Neck: supple, no meningismus. No periorbital edema.

ASSESSMENT:
Acute Otitis Media (AOM) — [unilateral: right / left] [bilateral] (ICD-10: H66.001 / H66.002 / H66.003)
[Severity: mild / moderate-severe based on: fever >39C, severe otalgia, bilateral AOM in child <2yo]

PLAN:
[TREATMENT — select applicable based on AAP 2022 guidelines:]

Option A — Antibiotic treatment initiated:
Amoxicillin [90 mg/kg/day divided BID x 10 days (age <2 or severe) / x 5-7 days (age 2+ mild-moderate)]
[Amoxicillin-clavulanate if penicillin tolerant but prior treatment failure or recurrent AOM]
[Cefdinir / Cefuroxime if penicillin allergy — non-anaphylactic]
[Ceftriaxone IM x 1-3 days if vomiting or severe allergy]

Option B — Observation with safety net prescription:
Observation appropriate (age 2+, unilateral, mild symptoms, reliable follow-up).
Prescription provided — fill only if symptoms worsen or do not improve in 48-72 hours.

Pain management: Ibuprofen [10 mg/kg/dose q6-8h PRN] or Acetaminophen [15 mg/kg/dose q4-6h PRN] for ear pain and fever.
No otic analgesic drops (anesthetic ear drops) if TM perforation possible.

RETURN PRECAUTIONS:
Return to clinic or seek care if: worsening ear pain, new fever or fever >72h, symptoms not improving after 48-72h of antibiotics, neck stiffness, facial swelling, new rash, hearing loss, or any parental concern.

FOLLOW-UP:
Recheck if: [symptoms persist after antibiotic course] / [bilateral AOM in child <2] / [recurrent AOM — consider audiology and ENT referral after 3+ episodes in 6 months or 4+ in 12 months].

Provider: [YOUR NAME, DEGREE]
Date: [DATE]
```

---

## Tips for managing your dot phrase library in Cerner

- **Naming system matters.** Use a consistent prefix so all your phrases group together. Everything starting with `wc` will list together, `ac` together, etc.
- **Keep a backup.** Copy your phrase text into a personal document (Word or Notes). Cerner My AutoText is user-specific and does not transfer between installations on PCS.
- **Update after guideline changes.** AAP and ACIP guidelines update regularly. Budget 30 minutes at the start of each year to review and update your acute visit and vaccine phrases.
- **Build once, use forever.** The biggest return on investment is the well-child visit series — build all 14 age-specific phrases in one sitting and you'll save hours every week.
- **Share with caution.** My AutoText phrases are personal and not automatically shared across a clinic. If your team wants shared phrases, work with your local Cerner administrator about clinic-wide order sets or documentation templates instead.
