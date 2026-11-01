# Revised project plan

## Project-level logic

1. **Freeze the question and scope.** Treat `hotel` as an indicator for the two observed properties. The target is a conditional association with ADR, not a causal effect and not cancellation prediction.
2. **Freeze the cleaning rules.** The Rmd reproduces the supplied 73,004-row clean data and then removes the 31 zero-recorded-guest records, leaving 72,973 observations. The 13 ADR-at-most-one records remain pending a separate documented decision.
3. **Align every section.** B's introduction, A's data description, C's model, and D's interaction figure must use the same population, response, predictor definitions, reference levels, and wording about the two properties.
4. **Submit reproducibly.** Knit the Rmd from the original CSV, compare the PDF's numbers and figures with the rendered output, and place original/cleaned data in the required U of T OneDrive link.

## C lead checklist

1. Confirm the working formula and the inclusion of arrival year with B and A.
2. Obtain A's written rationale for each cleaning decision; preserve the executable R code already in the Rmd.
3. Record the adopted rule that removes the 31 zero-recorded-guest records and ensure A reports the same rule and row count.
4. Fit the preliminary model and report all coefficient estimates with standard errors and 95% confidence intervals.
5. Interpret the main lead-time coefficient, the interaction, and the property-specific slopes using conditional-association language.
6. Assess linearity/mean structure, constant variance, normality, uncorrelated errors, and unusual observations using the saved diagnostic grids.
7. Do not correct assumption violations in Part 1. Put transformations, nonlinear terms, variance handling, and sensitivity analysis into the plan for Part 2.
8. Get B's actual literature result for the required "expected or surprising" comparison.
9. Keep the Preliminary Results section at 400 words or fewer, counting table and figure captions.
10. Have B review C's wording and numbers; then verify the final proposal against a fresh knit.

## Part 2 direction after Part 1

After the proposal is submitted and the cleaning rules are frozen, investigate a transformation of ADR, nonlinear lead-time terms, the variance structure, time/property clustering, influential observations, and predictor selection. Any revised model should be justified by the research question and diagnostics, compared with the preliminary specification, and accompanied by sensitivity analyses rather than automatic deletion of unusual rows.
