# Contributing

Thanks for looking. This is an open research hypothesis, and the whole point is to
be corrected in public.

## Ground rules

1. **Only real citations.** Every empirical statement needs a verifiable source —
   PubMed ID, clinicaltrials.gov ID, DOI, or a direct journal/preprint URL.
2. **No medical advice, no treatment protocols, no dosing.** This is basic research.
   See [`DISCLAIMER.md`](DISCLAIMER.md).
3. **Contradicting evidence is welcome.** If a claim is wrong, the best contribution
   is the citation that shows it.
4. **Do not self-promote a claim's status.** Status is maintained through independent
   literature review; open an issue or PR with the sources and let the review set it.

## Claim files

One Markdown file per claim at `claims/C###-short-slug.md`, with YAML front matter.
Copy [`claims/_TEMPLATE.md`](claims/_TEMPLATE.md):

```yaml
---
id: C001
claim: "one-sentence claim exactly as presented"
status: supported | partially-supported | contradicted | unverified | hypothesis
evidence_tier: human-rct | human-phase1-2 | animal | in-vitro | theoretical
sources:
  - title: ...
    url: https://pubmed.ncbi.nlm.nih.gov/...   # or clinicaltrials.gov / DOI
    note: what it actually shows
verified_by: <reviewer>
verified_on: YYYY-MM-DD
medical_claim_flag: true | false
---
```

The body holds a short rationale and caveats. Add the claim to
[`claims/INDEX.md`](claims/INDEX.md) (id, claim, status, tier). Nothing shows as
`supported` until its file has been filled in by literature review.
