# AGU Compliance

Use for submission audits, required summaries, figures, supporting information, and Open Research. Treat the tables below as a dated policy snapshot, not permanent rules. When an item affects submission, open the linked official source and report the verification date. Treat journal or article-type instructions as higher priority than AGU-wide guidance.

Policy snapshot checked: 2026-07-14.

## Rule classes and source keys

- **Required:** explicit submission requirement in an official AGU source.
- **Conditional:** required only for a named journal, article type, object, or circumstance.
- **Guidance:** writing or accessibility practice rather than a universal submission gate.

| Key | Official source | Use for | Checked |
|---|---|---|---|
| `TG` | [Text & Graphics Requirements](https://www.agu.org/publications/authors/journals/text-graphics-requirements) | Manuscript order, Key Points, Abstract, PLS, length, text and figures | 2026-07-14 |
| `PLS` | [Plain Language Summary](https://www.agu.org/publications/authors/journals/plain-language-summary) | PLS audience, structure, length, and journal list | 2026-07-14 |
| `SC` | [Journals Submission Checklists](https://www.agu.org/publications/authors/journals/submission-checklists) | Submission-level cross-checks and journal-specific requirements | 2026-07-14 |
| `DS` | [Data and Software for Authors](https://www.agu.org/publications/authors/journals/data-software-for-authors) | Repositories, Availability Statements, preservation, and citation | 2026-07-14 |
| `SI` | [Supporting Information](https://www.agu.org/publications/authors/journals/supporting-information) | Allowed role and contents of supporting information | 2026-07-14 |

## AGU-wide manuscript checks

| Check | Class | Scope | Source |
|---|---|---|---|
| Provide one to three Key Points; make each a complete thought, at most 140 characters, with no abbreviations. | Required | AGU journal manuscripts | `TG` |
| Use a one-paragraph Abstract of fewer than 250 words; use fewer than 150 words for GRL. Define abbreviations and omit figure/table mentions. | Required | AGU journals; GRL exception | `TG` |
| Arrange title page, Key Points, Abstract, conditional PLS, keywords, text, acknowledgments, Open Research, references, tables, and figures in the stated order. | Required | Initial submission | `TG` |
| Ensure every in-text literature citation resolves to a reference entry and every listed reference is cited in the manuscript or designated supporting-information reference section. | Required | References | `TG`, `SI` |
| Disclose affiliations or employment that could be perceived as conflicts in the acknowledgments and cover letter. | Conditional | When such a conflict may exist | `TG` |

## Plain Language Summary

- **Required (`TG`, `PLS`):** use one paragraph of no more than 200 words and remove jargon, acronyms, equations, and technical information unfamiliar outside the discipline.
- **Required journals among supported modes (`PLS`):** AGU Advances, Geophysical Research Letters, and Space Weather.
- **Optional but strongly encouraged under current AGU-wide guidance (`PLS`):** JGR: Space Physics, Earth and Space Science, and Radio Science, unless their current journal or article-type instructions say otherwise.
- **Audience guidance (`PLS`):** write for readers outside the subfield at an undergraduate level of scientific understanding. Cover what was studied, what was learned, and why it matters; do not merely simplify the Abstract sentence by sentence.

## GRL-specific checks

- Abstract under 150 words (`TG`, required).
- Research Letter no more than 12 publication units (`TG`, required).
- Central advance is timely, broadly consequential, and visible early (editorial framing; verify current GRL criteria when used).

## Figures and supporting information

- Cite figures in numerical order; use consistent panel labels (`TG`).
- Define quantities, units, scales, coordinates, colors, lines, symbols, data/model sources, and uncertainty (`TG`).
- Do not rely on color alone; avoid misleading interpolation or indistinguishable missing and zero values (`TG`, accessibility guidance).
- Keep discussion and key analysis out of supporting information (`SI`, required).
- Do not place data or software in supporting information as the preservation route; deposit them in an appropriate repository (`SI`, `DS`, required).

## Open Research

Check `what | purpose | repository | DOI or persistent URL | version | license/access | reference citation`.

- Make underlying data and software or code needed to understand, evaluate, and build upon the work available at peer review and publication (`DS`, required).
- Put an Availability Statement in a separate paragraph of the Open Research section (`DS`, required).
- Deposit research objects in a trusted repository, preferably with a DOI; link to the specific object rather than a repository home page (`DS`, required/guidance).
- Cite DOI-bearing data and software in References; include object type, repository, and version when available (`DS`, required).
- For software, distinguish the preserved release from the active development platform and state the version, access conditions, and license (`DS`, conditional).
- Do not invent identifiers or use “available upon request” or supporting information as the default preservation route (`DS`, required).

## Audit output

Use `pass` only when supplied material is checkable, `warn` for a conditional item, unverified current rule, or likely editorial risk, and `fail` for a missing required element. Put the applicable source key in every finding; include the live link and current verification date when the audit will be used for submission.

| Item | Status | Issue | Fix | Source |
|---|---|---|---|---|
| Journal fit and length | pass/warn/fail |  |  |  |
| Key Points and Abstract | pass/warn/fail |  |  |  |
| Plain Language Summary | pass/warn/fail |  |  |  |
| Figures, citations, and supporting information | pass/warn/fail |  |  |  |
| Open Research | pass/warn/fail |  |  |  |
