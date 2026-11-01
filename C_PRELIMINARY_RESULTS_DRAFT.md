# Preliminary Results

We fitted a preliminary multiple linear regression using 72,973 completed bookings. The model included the 14 predictors described in the Data Description and a lead-time-by-hotel interaction, allowing the association between lead time and mean ADR to differ between the two hotels.

**Model table caption.** Preliminary multiple linear regression estimates for ADR, with standard errors and 95% confidence intervals.

For the City Hotel, one additional day of lead time was associated with a 0.0944-euro decrease in mean ADR (95% CI: -0.0979, -0.0909), holding the other predictors fixed. The lead-time-by-hotel interaction estimate was 0.0551 euros (95% CI: 0.0498, 0.0604), giving a Resort Hotel slope of -0.0393 euros per day. Longer lead times were associated with lower ADR at both hotels, but the negative association was weaker at the Resort Hotel. The interaction confidence interval did not contain zero, providing evidence that the slopes differed between the hotels. This difference was consistent with Abrate et al. (2012), who found that inter-temporal hotel pricing varies with hotel and customer characteristics. The adjusted R-squared was 0.5823. 

**Condition figure captions.** Conditional mean response check. Pairwise plots of the numerical predictors.

The observed-versus-fitted plot shows systematic departures from the reference line. The pairwise plots do not show strong curved relationships among the numerical predictors, although several count predictors are concentrated at small values. Therefore, the conditional mean response condition is questionable, while the conditional mean predictor condition appears reasonable for the numerical predictors.

**Residual figure captions.** Residuals versus fitted ADR and lead time, and the normal Q-Q plot. Residuals versus weekend nights, weekday nights, and adults. Residuals versus children and special requests, and by hotel. Residuals by arrival month, meal plan, and market segment. Residuals by customer type and reserved room type. Residuals by repeat-guest and domestic status.

The residuals-versus-fitted and residuals-versus-lead-time plots show systematic patterns and changing spread, so the linearity and constant variance assumptions are questionable. The remaining residual plots are generally centered near zero, although discrete predictors form bands and some categories have different spreads. The Q-Q plot departs substantially from the line in both tails, so normality is not reasonable. Group or repeat bookings may produce related errors, but the data do not contain enough identifying information to verify the uncorrelated-errors assumption. Following the Part 1 instructions, we identify these violations without correcting them.
