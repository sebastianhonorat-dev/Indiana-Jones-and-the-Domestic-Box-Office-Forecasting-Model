# Research Findings
### 1. Interaction effects matter a LOT.

One paper (Karniouchina, 2011) repeatedly found:
star buzz × movie buzz interaction terms were important.

**Meaning:**
a famous actor alone isn’t enough.
A buzzy movie alone isn’t enough.
Together they amplify each other.

### 2. Valence underperformed compared to volume.

This keeps showing up in movie literature (Karniouchina, 2011; Kazi, 2016).

Papers says:

sentiment affected buzz volume indirectly
but not revenue directly

Meaning:
people talking may matter more than whether they’re mildly positive or negative.

### 3. Industry behavior itself adapts to expected demand.

A paper (Karniouchina, 2011) found distributors allocated FEWER opening screens to ultra-buzzy movies sometimes.

Why? 

The author assume distributor expected consumers to “go the extra mile” to see those movies anyway.

### 4. High entropy strengthened the effect of WOM on sales.

Meaning:
people trusted ratings MORE when reviews looked naturally mixed (Lee et al., 2017).

They also found average numeric ratings alone were weak/non-significant.

But:
rating × entropy interaction mattered.

The paper argues people EXPECT disagreement for movies because movies are 'preference goods.'

### 5. text and stars are NOT interchangeable.

A paper (Lee et al., 2017) found numeric ratings and actual text sentiment distributions were DIFFERENT.

This is huge because users normally rate similiarly to displayed average rating, but they express more nuanced feelings when writing text.

Someone may give a movie with an average rathing of 9.5, a 9/10 but write:

* “great visuals but weak ending”
* “fun but overrated”

### 6. Sequels decay faster

Sequels have stronger first weeks but worse retention afterward

Meaning:
they pull demand forward.

A paper (Dhar et al., 2011) calls this 'front loading.'

### 7. Historical entity performance is probably one of the strongest pre-release signal families
Their best features (Ahmed et al., 2019) were basically:
* prior actor success
* prior director success
* prior genre success
* experience metrics

That aligns with industry intuition too.

### 8. First-weekend behavior differed MORE strongly across movie slices than total gross behavior.

Their theory (Antipov & Pokryshevskaya, 2011):

* studios can adjust marketing later to compensate for weak openings.

Meaning: opening weekend may reflect intrinsic positioning more directly, while long-run revenue becomes more dynamic.

### 9. Informative movie titles help under-promoted movies significantly.

But once marketing becomes large enough or familiar IP is involved, title quality matters much less.

Example:

* “Paranormal Activity”
* “My Big Fat Greek Wedding”
* “Night of the Living Dead”

These titles instantly communicate tone, genre, premise, and vibe

While something like:

* “Lucy”
* “Joe”
* “Broken”

tells you almost nothing.

The paper (Bae & Kim, 2019) also found title effects were strongest during opening week and faded quickly afterward.

### 10. Studios don’t release movies randomly.

A paper (Belleflamme & Paolini, 2018) argues:
high-budget movies intentionally cluster near demand peaks:

* summer
* holidays
* Thanksgiving
* Memorial Day
* Christmas

BUT they avoid releasing DIRECTLY against similar genre competitors.

Example:
Two R-rated horror films releasing together may cannibalize each other heavily.

But:
a Pixar film and horror film may coexist fine.

Also, lower budger films may avoid those demand peak windows because they would get crushed by competition.

### 11. Ex ante vs Ex post predictors

This paper (Brewer et al., 2009) seperates infomation that is available before release and after release.

Their strongest ex ante predictors:

* production budget
* sequel/pre-existing audience
* critic reviews
* summer release
* holiday release

Their strongest ex post predictors:

* screen count
* word of mouth
* awards
* stars
* audience scores

Their ex ante model had:
Adjusted R² ≈ 0.41

Their stronger ex post model reached:
Adjusted R² ≈ 0.65

### 12. Pre-release prediction is MUCH harder

They (Dursun Delen & Sharda, 2008) explicitly note:
once opening weekend arrives, prediction becomes far easier.

The hard problem is pre-release uncertainty.

### 13. Effects differ across revenue quantiles.

According to Feng & Sharma (2016), features matter differently for:

* bombs
* mid-tier films
* blockbusters

My tree-model intuition is probably right, so XGB may implicitly capture these nonlinear regimes already.

### 14. Audiences behaved differently toward imported vs domestic films.

Different audience ecosystems may obey different rules (Feng & Sharma, 2016).

### 15. Summer movies don’t only perform better because more people go to theaters.

They also perform better because studios intentionally save their strongest movies for summer.

It means:
release timing is partially a SIGNAL OF STUDIO CONFIDENCE.

The paper (Einav, 2007) argues distributors often avoid placing strong movies into weak periods even if competition is lighter.

---
## References

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