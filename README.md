# ICU Pre-Rounding Simulator

A free, browser-based chart-review simulator for teaching critical care pre-rounding to interns and students. One HTML file, no installation, no accounts, no network access, no patient data. Every patient is fictional.

**Open it here:** https://henriquepuls.github.io/icu-prerounding-simulator/

Or download `index.html` and open it in any browser. Progress saves in the browser on the computer where you play.

## What it does

The learner is the intern. Sign-out ended at 06:30 and rounds start soon. For each patient the learner:

1. Reads a mock chart with nine tabs: overview, overnight events, vitals, respiratory and ventilator, labs, medications, lines and intake and output, microbiology and imaging, notes.
2. Fills in a systems-based pre-rounding template (neuro to skin) that becomes both the presentation and the note, and runs the ICU Liberation (ABCDEF) checklist.
3. Clicks "I'm done: check my work". The simulator scans the template text for each gold-standard item, pre-checks what it finds, and lets the learner correct the scan in both directions.
4. Sees a score, capture by organ system, and for every missed item a short explanation of why it matters.

A countdown timer runs while a chart is open. A facilitator view (click the link on the home screen twice) reveals the gold-standard checklist with teaching rationale, the planted pitfalls, teaching pearls, discussion questions, and a model rounds presentation for each case.

## The cases

| Bed | Patient | Problem |
| --- | --- | --- |
| MICU 12 | Mills, Dorothy, 68 F | Multifocal pneumonia, septic shock on norepinephrine |
| MICU 4 | Webb, Marcus, 54 M | Out-of-hospital VF arrest after PCI, intubated, active fever prevention |
| MICU 7 | Ortiz, Raymond, 61 M | COPD exacerbation with hypercapnic respiratory failure, intubated |
| MICU 9 | Herrera, Luis, 49 M | Upper GI bleed with alcohol-related cirrhosis |

Each case carries deliberately planted findings that a strong pre-round catches. The facilitator view lists them. Learners get more from the cases if they do not read that view first.

## The five-step framework

The home screen and the "5-Step Guide" button teach the framework the simulator is built around:

1. **Triage your list.** Who got worse, who is new, what happened overnight.
2. **Chart check.** Events, vital sign trends, ventilator and gases, labs, drips and the medication record, fluid balance.
3. **Bedside look.** The patient, the monitor, the pumps, the ventilator. The simulator cannot replace this step.
4. **Assessment and plan by system.** Neuro to skin, one line each. It becomes the note.
5. **ICU Liberation checklist.** The ABCDEF bundle, run before you present.

The framework is adapted from @defineshock.

## Running a workshop

The format that was piloted with one emergency medicine intern class fits in one hour:

- 10 minutes: the five-step framework.
- Two timed 10-minute cases (septic shock, then ventilated COPD), each followed by a facilitated group debrief using the facilitator view.

Learners can work on their own laptops or in pairs. No network is needed once the file is open.

## Adapting it

The whole simulator is one file. Cases live in the `CASES` array in the inline script, the template fields in `TPL_FIELDS`, the checklist scanning keywords in `KEYWORDS`, and the ICU Liberation items in `ABC_ITEMS`. Edit them in any text editor to change the cases, add your own, or translate the interface.

The application was built in a few days by a physician with no coding experience using a large language model coding harness. Educators can reproduce the method to create tools for their own learners and environments.

## Author and license

Created by Henrique A. Puls, MD, Division of Resuscitation and Emergency Critical Care, Department of Emergency Medicine, Prisma Health Upstate and University of South Carolina School of Medicine Greenville.

Licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). You can use, share, and adapt it for any purpose, including commercially, as long as you credit the author. See `LICENSE`.
