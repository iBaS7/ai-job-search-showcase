# Visa and sponsorship: read the sentence, not the keyword

**Problem.** Searching postings for "visa sponsorship" also returns postings that refuse it. A keyword match counted them as supportive.

| Posting sentence | Verdict |
|---|---|
| "We can offer visa sponsorship and a relocation package." | Pass; quote it. |
| "Relocation packages and visa sponsorship where necessary." | Conditional; mark as unverified. |
| "We do not offer visa sponsorship for this role." | Fail. |
| "Candidates must already have the right to work without sponsorship." | Fail. |
| (no mention) | Fail for roles abroad that require explicit support; otherwise unverified. |

**Procedure.** Read the full sentence and its neighbours. Quote the sentence relied on in the fit report. Never summarise a refusal as support.

I proposed a generic version of this rule to the upstream project's Eligibility Gate: [discussion #894](https://github.com/ai-job-search-dev/ai-job-search/discussions/894) and [pull request #895](https://github.com/ai-job-search-dev/ai-job-search/pull/895) (open at the time of writing; the maintainers decide whether it fits the project).
