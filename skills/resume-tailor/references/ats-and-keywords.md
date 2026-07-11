# ATS & keyword reference

Read this when assembling a tailored resume (resume-tailor Step 4). It covers
two things: keeping the file machine-readable, and weaving in the job's keywords
without lying.

## Applicant Tracking Systems (ATS) — what breaks parsing

Most mid-to-large employers screen resumes through an ATS before a human reads
them. To stay parseable:

- **Single column, no tables** for the body. Multi-column layouts and text boxes
  scramble reading order. (A clean Markdown → Docs export is safe.)
- **Standard section headings**: `Experience`, `Education`, `Skills`,
  `Projects`, `Certifications`. Don't get creative ("Where I've Made Impact"
  can be missed).
- **No text inside images, headers/footers, or graphics** — many parsers skip
  them entirely. Never put contact info only in a header.
- **Real dates** in a consistent format (`Mon YYYY – Mon YYYY`).
- **Spell out then abbreviate** the first time: `Electronic Health Record (EHR)`,
  so both the phrase and the acronym match a search.
- **Common file types**: `.docx` and text-based `.pdf` parse best.

## Keyword strategy — match without fabricating

The goal is that a recruiter (and their search) sees their own language
reflected back, using the user's *real* experience.

1. From the job description, list the recurring nouns and skills (tools,
   methods, domains, certifications). These are the target keywords.
2. For each keyword, find the closest **true** evidence in `achievements.md`.
   - Exact match → use their exact term.
   - Synonym the user actually did → adopt the job's wording
     (e.g. user wrote "signal processing", job says "DSP" → use "DSP" if it's
     genuinely the same work).
   - No real evidence → **do not add it.** Note it as a gap instead.
3. Place keywords where they carry weight: the summary line, a dedicated Skills
   section, and inside achievement bullets (not a hidden keyword-stuffed block —
   modern ATS and every human penalize that).
4. Prefer keywords in context: "Reduced prior-auth turnaround 40% by automating
   HL7 v2 message routing" beats a bare "HL7 v2" in a list.

## Truthfulness rules (non-negotiable)

- Never invent titles, employers, dates, degrees, or metrics.
- Never claim a tool/skill with no real basis, even to match a must-have.
- Reframing and emphasis are fine; fabrication is not. When unsure, flag it to
  the user rather than guessing.

## Quick pre-send checklist

- [ ] One column, standard headings, real dates
- [ ] Top third mirrors the job title and top 3 requirements
- [ ] Every must-have is either evidenced or listed in the honesty gap-check
- [ ] Acronyms spelled out once
- [ ] No fabricated numbers, tools, or titles
- [ ] Exports cleanly to `.docx`/text `.pdf`
