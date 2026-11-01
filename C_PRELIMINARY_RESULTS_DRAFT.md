# C section: preliminary results draft

## Proposed text for the proposal

We fitted a preliminary multiple linear regression to 72,973 non-cancelled bookings with positive ADR and at least one recorded guest. The model included lead time, hotel property, arrival year and month, weekend and weekday nights, adults, children, meal plan, reserved room type, market segment, and customer type, together with the lead-time-by-hotel interaction. With the City Hotel as the reference, one additional lead-time day was associated with a 0.1207-euro lower mean ADR (95% CI: -0.1242, -0.1172), holding the remaining predictors fixed. The interaction estimate was 0.0607 euros (95% CI: 0.0555, 0.0658), so the corresponding Resort Hotel slope was -0.0600 euros per day. Thus, longer lead times were conditionally associated with lower ADR at both properties, but the negative association was weaker at the Resort Hotel. These are associations, not causal effects. The model had an adjusted R-squared of 0.6076 and a residual standard error of 29.55 euros.

The residual-versus-fitted plot showed a pronounced change in spread and systematic structure, so constant variance and the linear mean specification were not reasonable. The residual histogram was right-skewed, and the QQ plot departed strongly from the reference line in both tails, especially the upper tail, so normality was not reasonable. Residuals also showed long runs over calendar/source order and strong positive autocorrelation, making uncorrelated errors implausible. Several large standardized residuals and a small high-leverage group require source-record checks but were not removed automatically. Following the Part 1 instructions, we diagnose these violations without correcting them at this stage.

**Table 1 caption.** Preliminary multiple linear regression estimates for ADR (euros per night), with standard errors and 95% confidence intervals; reference levels are City Hotel, 2015, January, BB meal, room A, Online TA, and Transient customer.

**Figure 1 caption.** Preliminary diagnostics for the ADR model: standardized residuals versus fitted ADR, residual histogram, and normal QQ plot. The changing spread, right skew, and tail departures indicate violations of constant variance and normality.

## Required literature handoff before submission

Add one sentence comparing the lead-time result with one of B's three cited papers. Do not invent this comparison. Suggested structure: "This [agrees/contrasts] with [Author, year], who reported [specific relevant result], and was [expected/surprising] because [brief reason]."

## Numerical checkpoints

- City Hotel lead-time slope: -0.1207; 95% CI [-0.1242, -0.1172].
- Lead-time-by-Resort-Hotel interaction: 0.0607; 95% CI [0.0555, 0.0658].
- Resort Hotel lead-time slope: -0.0600.
- Residual standard error: 29.55 euros.
- R-squared: 0.6078; adjusted R-squared: 0.6076.
- Observations: 72,973.

The proposal's 400-word limit includes table and figure captions. Recount after adding the literature sentence or changing any caption.

