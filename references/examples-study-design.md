# Data and Methods Writing Patterns

Use these structure-only patterns for Data and Methods. Replace every bracketed field with author-provided or verified content. Do not let a pattern supply a missing instrument property, parameter, uncertainty, or validation result.

## Data

`We use [source/instrument/product] measurements of [quantity] over [verified range] to [role in the argument]. The data have [cadence/resolution/coverage] and are expressed in [coordinates and units]. We retain observations satisfying [quality or selection criteria] and treat [calibration, response, contamination, or coverage issue] using [verified procedure]. These measurements constrain [claim] but do not directly determine [boundary].`

`[Derived quantity] is calculated from [inputs] using [verified method]. It serves as [proxy/diagnostic/outcome], rather than a direct measurement of [distinction]. Its uncertainty reflects [supplied sources].`

## Event or observational analysis

`We identify [events/intervals] using [criteria]. For each interval, we calculate [derived quantities] from [inputs] and compare [diagnostic A] with [diagnostic B] over [coordinates/scales]. This comparison tests [specific hypothesis]. Uncertainty is estimated from [method], and intervals affected by [failure condition] are excluded or flagged.`

## Statistical analysis

`The sample contains [verified population] selected using [criteria]. We bin observations by [dimensions] and calculate [statistic] using [weighting/normalization]. We test robustness with [resampling, alternative thresholds, uncertainty propagation, or independent subset]. The sampling does not constrain [missing regime].`

## Numerical model or theory

`The model solves [governing system] with [included processes]. Initial and boundary conditions come from [source], while [parameters] are [measured/fitted/assumed] within [verified range]. We evaluate the model against [independent observations or benchmark] using [metric] and test sensitivity to [claim-critical assumptions].`

For theory, replace model setup with `assumptions -> derivation -> parameter regime -> limiting cases -> observable prediction`.

## Forecast or algorithm evaluation

`We predict [target] at [lead time] from [predictors]. Development uses [training design], while performance is evaluated on [independent test design] against [baseline]. We report [metrics] overall and for [relevant regimes] and examine missed events, false alarms, and [coverage/latency/threshold] limitations.`
