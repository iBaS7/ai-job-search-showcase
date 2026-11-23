# Evidence-based job applications with Claude Code

How I run a job search as a repeatable, checked process: research, fit evaluation, CV and cover letter tailored per posting, and verification, with me approving and submitting every application myself.

I use the open-source [AI Job Search](https://github.com/ai-job-search-dev/ai-job-search) framework (MIT, see [NOTICE.md](NOTICE.md)) with Claude Code. This repository is not that framework and contains no personal data. It shows the method and the rules I added on top.

## The workflow

1. **Evaluate fit first.** Each posting is scored against my profile before any document is written. Hard filters (location rules, visa and eligibility wording, mandatory language) run before scoring.
2. **Tailor from evidence.** Every CV bullet and cover-letter claim must trace to a documented experience in my own source documents. No invented skills, tools or numbers. If the source gives no figure, the document gives none.
3. **Verify mechanically.** CV compiles to exactly two pages, cover letter to one; the PDF text layer is extracted and checked the way an applicant-tracking system reads it; no orphaned headings at page breaks.
4. **Human in the loop.** Claude Code drafts and researches. I check the claims, decide what to say, and submit by hand. Automated submission is off.

## Rules I added (see [rules/](rules/))

- **Visa wording needs a negation check.** A keyword hit on "visa sponsorship" is not support; postings often say "we do not offer visa sponsorship". Read the sentence, quote it as evidence, treat conditional wording as unverified.
- **Do not volunteer gaps.** Before calling something a gap, search my source documents for evidence. Cover letters stay positive and factual; real gaps are reported to me in chat, not written into the letter.
- **Never name a tool I did not use.** A claim such as "built with X" appears only if I confirmed it.

## Worked example

[examples/evidence-mapping.md](examples/evidence-mapping.md) walks through one fictional posting: requirements, the evidence found, the resulting bullets, and what is deliberately left out.

## What this is not

Not a product and not the framework's author's work. It is documentation of how I operate a tool I did not build, with the corrections I made when its output over-claimed.
