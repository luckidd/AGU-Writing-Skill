# Section Writing Guide

Use this file to decide what each manuscript part must accomplish. Draft only from author-provided or verified evidence. Load only the matching pattern file when wording examples will materially help: [front matter](examples-front-matter.md), [study design](examples-study-design.md), [main text](examples-main-text.md), or [figures and Open Research](examples-figures-open-research.md).

## Title

### Purpose

Identify the physical system or quantity, the process or relationship, and the paper's distinctive contribution. A title should help the intended audience judge relevance without reading the abstract.

### Build it

1. Name the phenomenon, process, or product.
2. Add the physical regime, spatial domain, or application only when it narrows the claim.
3. Add the evidence or approach when it distinguishes the work.
4. Prefer a result-led title when the main finding is defensible; use a scope-led title when the paper presents data, methods, or an instrument.

### Avoid

- Empty openings such as `Study of`, `Investigation of`, or `Some results on`.
- Unsupported priority words such as `first`, `novel`, `unprecedented`, or `universal`.
- A list of missions that hides the scientific contribution.
- A causal title when the evidence supports only association.

### Check

Does the title match the strongest claim actually supported in Results and Discussion? Could a reader distinguish an event study, statistical result, method, and forecast product?

## Abstract

### Purpose

Allow a reader to judge the problem, approach, principal evidence, advance, and boundary without consulting the paper.

### Recommended moves

1. **Context:** one sentence defining the specific physical or operational problem.
2. **Gap:** name what is unresolved, unquantified, poorly constrained, or unavailable.
3. **Approach:** state the observations, model, theory, experiment, or validation design that addresses the gap.
4. **Results:** give two to four major findings, prioritizing quantitative results supplied by the author.
5. **Interpretation:** state the physical explanation at the level supported by the diagnostics.
6. **Implication and boundary:** state what changes and where the conclusion applies.

Compress context before compressing results. Do not turn the abstract into an introduction or a list of methods. Define abbreviations, avoid figure calls, and do not add citations unless formally necessary.

### Journal adaptation

- **GRL:** make the advance visible in the first half; minimize setup; remain under 150 words.
- **AGU Advances:** make the cross-disciplinary conceptual importance explicit without inflating the claim.
- **JGR: Space Physics:** include enough method and diagnostic detail to establish the evidence chain.
- **Space Weather:** state target, baseline or comparison, validation regime, performance, and practical implication.
- **Earth and Space Science / Radio Science:** emphasize validation, reproducibility, measurement or technical contribution.

### Check

Can every result sentence be traced to a supplied result? Are conditions, sample limits, uncertainty, and model dependence retained? Does the last sentence say more than “improves understanding”?

## Key Points

### Purpose

Present the paper's main results as self-contained, searchable statements understandable beyond the immediate specialty.

### Build them

- Use one point for the principal observed or modeled result.
- Use a second for the controlling process, diagnostic, or quantitative relationship.
- Use a third for the bounded scientific, modeling, data, or operational implication.

Each point should contain one claim. Use plain words instead of acronyms and avoid method-only statements unless the method itself is the contribution.

### Check

Do the points agree with the title, abstract, and conclusions? Are they results rather than background or promises? Verify current character limits in `agu-compliance.md` when auditing.

## Plain Language Summary

### Purpose

Explain the same study and broader relevance as the Abstract in a different language and tone. Write for readers outside the subfield at an undergraduate level of scientific understanding, not for specialists and not for an assumed expert-free general public.

### Recommended moves

1. **Topic overview:** introduce the phenomenon and why it matters in familiar terms.
2. **Paper overview:** state the question and describe the approach without instrument-heavy detail.
3. **Findings summary:** state what was learned, preserving the distinction between result and interpretation.
4. **Key takeaway:** explain the bounded scientific or societal relevance.

Use the minimum technical vocabulary needed to preserve the science and define unavoidable field-specific terms in place. For a submission-ready PLS, remove acronyms, equations, coordinate notation, channel labels, and specialist shorthand; expand an acronym into plain words rather than deleting its scientific role. Explain potentially ambiguous scientific words such as `regime`, `signal`, `uncertainty`, and `mean` in ordinary language. Do not translate or simplify the Abstract sentence by sentence.

Keep the PLS to one paragraph of no more than 200 words when preparing submission-ready text, and verify the current journal requirement in `agu-compliance.md`.

### Check

Could an undergraduate-level reader outside the subfield explain what was studied, what was learned, and why it matters? Is the distinction between observation and interpretation still visible? Does the text avoid claiming a broader public or operational benefit that the evidence does not establish?

## Introduction

### Purpose

Lead from the broad system to one answerable gap and show why the chosen evidence can resolve it.

### Paragraph architecture

1. **System and significance:** establish the relevant solar, heliospheric, magnetospheric, ionospheric, thermospheric, radio-science, or operational context.
2. **Process framework:** organize known processes by mechanism or scientific question, not as a chronological citation list.
3. **Current evidence and limitation:** state what observations, models, or theory already establish and what they cannot distinguish.
4. **Precise gap:** identify a mechanism, quantification, coverage, method, validation, or application gap.
5. **Present study:** specify data or method, regime or sample, question, and bounded contribution.

Not every paper needs five paragraphs. Combine adjacent jobs for GRL; separate them when JGR reproducibility or AGU Advances breadth requires more context.

### Check

- Does every background paragraph narrow toward the stated gap?
- Is the gap specific enough to be answered by the study?
- Are citations grouped by scientific role?
- Does the final paragraph state what is tested or quantified rather than promise broad understanding?

## Data

### Purpose

Show what was measured or obtained, why it is suitable, how it supports the argument, and what limits its interpretation.

### For each source, report as relevant

- Mission, instrument, network, database, simulation product, or experiment.
- Measured or derived quantity, energy/frequency range, cadence, resolution, sensitivity, and units.
- Spatial and coordinate coverage; time range; event or sample-selection role.
- Calibration, screening, quality flags, gaps, contamination, response, or version.
- Role in the paper: context, driver, constraint, diagnostic, validation, or outcome.

Separate direct measurements from derived quantities and proxies. Do not treat an integral channel as a narrow differential measurement or infer an unmeasured region without mapping or model support.

### Check

Could a reader determine which dataset supports each main claim? Are access and citation details handled separately in Open Research?

## Methods

### Purpose

Make the inference reproducible and show why the selected analysis can answer the stated question.

### Choose the relevant sequence

- **Event/observational:** selection -> preprocessing -> derived quantities -> conjunction or comparison -> uncertainty.
- **Statistical:** coverage -> inclusion/exclusion -> binning or normalization -> statistical test -> robustness and bias.
- **Numerical model:** governing equations -> process terms -> initial/boundary conditions -> inputs and parameters -> numerical setup -> validation and sensitivity.
- **Theory:** assumptions -> derivation -> parameter regime -> limiting cases -> observable prediction.
- **Instrument/algorithm:** measurement principle -> response or algorithm -> calibration/training -> independent validation -> uncertainty and failure regime.
- **Data assimilation:** state variables -> observations and operators -> prior/error assumptions -> assimilation cycle -> independent evaluation.
- **Forecast/application:** target and lead time -> predictors -> baseline -> train/validation/test separation -> metrics -> operating threshold and failure analysis.

State where key parameters come from: observation, fit, literature, calibration, or assumption. Distinguish uncertainty, sensitivity, and validation. Describe software or model versions when results depend on them.

### Check

Could another researcher reproduce the analysis or identify what prevents reproduction? Is every parameter central to the conclusion defined and tested or justified?

## Results

### Purpose

Establish findings in the order needed to answer the research question, using figures and quantitative evidence without narrating panels mechanically.

### Paragraph architecture

1. State one result claim.
2. Give quantitative or otherwise specific evidence and its regime.
3. Relate it to an independent diagnostic, comparison, or test.
4. State only the immediate physical meaning supported by the result.
5. End with a boundary or the reason for the next analysis.

Use an event overview to establish timing and context, not to claim a final mechanism. Distinguish observations, derived products, model output, and sensitivity tests. Use statistical significance only with effect size and physical relevance when supplied.

### Check

- Does each paragraph state its conclusion before details?
- Are numbers, ranges, coordinates, and uncertainty preserved?
- Is a correlation described as association unless causal evidence is supplied?
- Does the figure actually contain every visual fact invoked?

## Discussion

### Purpose

Explain what the results mean, how strongly they support a mechanism or application, how they compare with prior work, and where the conclusion stops.

### Paragraph architecture

1. **Central interpretation:** answer the research question using calibrated language.
2. **Evidence synthesis:** combine independent results instead of repeating them.
3. **Competing explanations:** state material alternatives and the diagnostics that support or fail to exclude them.
4. **Prior work:** explain agreement, extension, difference, or changed boundary.
5. **Limitations:** connect each limitation to the claim it affects.
6. **Implication:** state what should change in understanding, modeling, measurement, or operations.

For forecasts, distinguish retrospective fit, hindcast, and genuine forecast; report baseline comparison, independent validation, failures, coverage, latency, and threshold dependence when supplied.

### Check

Does the Discussion interpret rather than restate Results? Are alternatives treated in proportion to their effect on the conclusion? Are limitations specific rather than ceremonial?

## Conclusions

### Purpose

Provide the smallest complete statement of what was learned and under what conditions.

### Structure

`objective -> evidence/approach -> two to five supported findings -> bounded implication -> unresolved need`

For numbered findings, include result, regime, and physical meaning in each item. Do not introduce a new mechanism, citation-dependent argument, or result. Avoid generic endings.

### Check

Do the conclusions match the abstract and Key Points in strength and scope? Is future work linked to a stated limitation rather than added as a generic sentence?

## Figure Captions

### Purpose

Let readers identify the plotted evidence without searching Methods while leaving broad interpretation to the main text.

### Include as relevant

- Figure purpose and panel definitions.
- Quantities, units, scales, coordinate systems, intervals, and regimes.
- Colors, lines, symbols, shading, thresholds, and reference levels.
- Observation, derived product, model run, or experiment source.
- Processing, normalization, uncertainty, and missing-data treatment needed to read the figure.

### Check

Are panels labeled consistently? Can observation and model be distinguished? Does the caption avoid conclusions not supported in the text?

## Open Research

### Purpose

Tell readers what data and software support the work, their purpose, where the preserved objects are located, and how they can be accessed and cited.

Collect: object type, role, repository, DOI or persistent URL, version, license/access conditions, and formal reference. Keep unknown details as placeholders and verify identifiers before submission.
