# Research Findings

## 1. Interaction Effects Matter Significantly

Karniouchina (2011) repeatedly found that interaction terms between *star buzz* and *movie buzz* were highly important predictors.

### Key Insight
A famous actor alone is not enough.  
A highly discussed movie alone is not enough.  

However, when both are present simultaneously, their effects amplify each other substantially.

This suggests that pre-release attention may behave multiplicatively rather than additively.

---

## 2. Buzz Volume Outperformed Sentiment Valence

Several papers (Karniouchina, 2011; Kazi, 2016) found that the *amount* of discussion surrounding a film was more predictive than whether discussions were slightly positive or negative.

### Key Insight
Sentiment primarily affected buzz volume indirectly rather than revenue directly.

This implies that audience engagement itself may matter more than mild variations in positivity or negativity.

---

## 3. Industry Behavior Adapts to Expected Demand

Karniouchina (2011) observed that distributors sometimes allocated *fewer* opening screens to extremely buzzy films.

### Proposed Explanation
Distributors may assume consumers are willing to “go the extra mile” to see highly anticipated films regardless of theater availability.

This suggests that release strategy itself may contain information about expected demand.

---

## 4. Review Entropy Strengthened WOM Effects

Lee et al. (2017) found that higher review entropy strengthened the impact of ratings on sales.

### Key Insight
Consumers appeared to trust ratings more when reviews showed natural disagreement.

Average ratings alone were often weak or statistically insignificant. However:

- `rating × entropy` interaction effects were important.

The paper argues that movies are “preference goods,” meaning audiences expect disagreement in opinions.

---

## 5. Numeric Ratings and Text Sentiment Are Not Equivalent

Lee et al. (2017) also found that numeric ratings and written review sentiment distributions behaved differently.

### Key Insight
Users often conform to visible average ratings numerically while expressing more nuanced opinions in text.

For example, a viewer may rate a movie highly while still writing:

- “Great visuals but weak ending”
- “Fun but overrated”

This suggests that textual sentiment may contain richer information than aggregate numeric scores alone.

---

## 6. Sequels Experience Faster Revenue Decay

Dhar et al. (2011) found that sequels tend to produce:

- stronger opening weekends,
- but weaker long-term retention.

### Key Insight
Sequels appear to pull demand forward into the earliest release window, a phenomenon described as **front loading**.

---

## 7. Historical Entity Performance Is a Strong Pre-Release Signal

Ahmed et al. (2019) found that many of the strongest predictive features were based on historical performance metrics, including:

- prior actor success,
- prior director success,
- prior genre success,
- and experience-related metrics.

### Key Insight
Historical performance appears to be one of the most reliable families of pre-release predictors.

---

## 8. Opening Weekend Behavior Varies More Across Film Segments

Antipov & Pokryshevskaya (2011) found that opening weekend performance differed more strongly across movie “slices” than total gross performance.

### Proposed Explanation
Studios can later adjust marketing strategies to compensate for weak openings.

This suggests:

- opening weekend may reflect intrinsic positioning more directly,
- while total gross becomes increasingly influenced by dynamic post-release adjustments.

---

## 9. Informative Titles Help Under-Promoted Films

Bae & Kim (2019) found that descriptive or informative titles significantly benefited films with weaker marketing support.

### Examples of Informative Titles
- *Paranormal Activity*
- *My Big Fat Greek Wedding*
- *Night of the Living Dead*

These titles immediately communicate genre, tone, or premise.

### Less Informative Examples
- *Lucy*
- *Joe*
- *Broken*

The paper also found that title effects were strongest during opening weekend and faded over time.

---

## 10. Studios Do Not Release Films Randomly

Belleflamme & Paolini (2018) argue that release timing reflects strategic positioning decisions.

### Observed Patterns
High-budget films cluster around demand peaks such as:

- summer,
- holidays,
- Thanksgiving,
- Memorial Day,
- and Christmas.

However, studios often avoid releasing directly against highly similar competitors.

### Example
Two R-rated horror films releasing simultaneously may heavily cannibalize each other, while a Pixar film and a horror film may coexist more effectively.

Lower-budget films may intentionally avoid peak windows due to competitive pressure.

---

## 11. Ex Ante vs Ex Post Prediction

Brewer et al. (2009) separated predictors into:

- **Ex ante predictors** (available before release),
- **Ex post predictors** (available after release).

### Strongest Ex Ante Predictors
- production budget,
- sequel or pre-existing audience,
- critic reviews,
- summer release,
- holiday release.

### Strongest Ex Post Predictors
- screen count,
- word of mouth,
- awards,
- stars,
- audience scores.

### Reported Performance
- Ex ante model: Adjusted R² ≈ 0.41
- Ex post model: Adjusted R² ≈ 0.65

### Key Insight
Prediction accuracy improves substantially once post-release information becomes available.

---

## 12. Pre-Release Prediction Is Substantially Harder

Delen & Sharda (2008) explicitly note that prediction becomes much easier once opening weekend data exists.

### Key Insight
The true challenge is modeling uncertainty *before* release.

---

## 13. Feature Effects Differ Across Revenue Quantiles

Feng & Sharma (2016) found that predictor importance varies across:

- bombs,
- mid-tier films,
- and blockbusters.

### Key Insight
Movie performance likely operates within nonlinear regimes rather than a single global relationship.

This supports the use of flexible models such as XGBoost that can capture heterogeneous effects implicitly.

---

## 14. Imported and Domestic Films Behave Differently

Feng & Sharma (2016) also found that imported and domestic films follow different audience dynamics.

### Key Insight
Different audience ecosystems may obey different predictive rules, suggesting that combining them may introduce noise into a unified model.

---

## 15. Release Timing May Signal Studio Confidence

Einav (2007) argues that summer movies do not outperform solely because more consumers attend theaters during summer.

### Key Insight
Studios intentionally reserve many of their strongest films for high-demand periods.

As a result, release timing itself may partially act as a signal of studio confidence in the film’s expected performance.

---

# References

Ahmed, U., Waqas, H., & Afzal, M. T. (2019). *Pre-production box-office success quotient forecasting*. Soft Computing, 24(9), 6635–6653. https://doi.org/10.1007/s00500-019-04303-w

Antipov, E., & Pokryshevskaya, E. (2011). *Accounting for latent classes in movie box office modeling*. Journal of Targeting, Measurement and Analysis for Marketing, 19(1), 3–10. https://doi.org/10.1057/jt.2011.3

Bae, G., & Kim, H. (2019). *The impact of movie titles on box office success*. Journal of Business Research, 103, 100–109. https://doi.org/10.1016/j.jbusres.2019.06.023

Belleflamme, P., & Paolini, D. (2018). *Strategic attractiveness and release decisions for cultural goods*. Journal of Economics & Management Strategy, 28(2), 198–224. https://doi.org/10.1111/jems.12280

Brewer, S. M., Kelley, J. M., & Jozefowicz, J. J. (2009). *A blueprint for success in the US film industry*. Applied Economics, 41(5), 589–606. https://doi.org/10.1080/00036840601007351

Dhar, T., Sun, G., & Weinberg, C. B. (2011). *The long-term box office performance of sequel movies*. Marketing Letters, 23(1), 13–29. https://doi.org/10.1007/s11002-011-9146-1

Delen, D., & Sharda, R. (2008). *Predicting the financial success of Hollywood movies using an information fusion approach*.

Einav, L. (2007). *Seasonality in the U.S. motion picture industry*. The RAND Journal of Economics, 38(1), 127–145. https://doi.org/10.1111/j.1756-2171.2007.tb00048.x

Feng, F., & Sharma, R. (2016). *Modeling the main determinants of movie sales: An econometric study of Chinese marketplace*. Journal of Reviews on Global Economics, 5, 190–209. https://doi.org/10.6000/1929-7092.2016.05.17

Karniouchina, E. V. (2011). *Impact of star and movie buzz on motion picture distribution and box office revenue*. International Journal of Research in Marketing, 28(1), 62–74. https://doi.org/10.1016/j.ijresmar.2010.10.001

Kazi, B. (2016). *Investigating the impact of firm-generated content on user-generated content and box office sales*. Carolina Digital Repository. https://cdr.lib.unc.edu/concern/honors_theses/1z40kx80t

Lee, J. H., Jung, S. H., & Park, J. (2017). *The role of entropy of review text sentiments on online WOM and movie box office sales*. Electronic Commerce Research and Applications, 22, 42–52. https://doi.org/10.1016/j.elerap.2017.03.001