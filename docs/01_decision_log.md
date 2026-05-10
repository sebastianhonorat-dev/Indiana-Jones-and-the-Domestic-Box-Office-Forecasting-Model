## Decisions

### 1. Scope Restriction: 2004–Present

Initially, I considered avoiding social media features such as tweet sentiment and discussion volume because films released before widespread social media adoption would be structurally disadvantaged in the dataset. My original goal was to identify more timeless signals of box office performance that could generalize across decades.

However, I now suspect that pre-social-media and post-social-media box office behavior may represent fundamentally different market dynamics rather than simply missing data. Modern films exist in an environment where online discourse, rapid consensus formation, and digital hype cycles significantly influence audience behavior.

Because of this, I decided to narrow the scope of the project to films released from 2004 onward. This date aligns with the availability of Google Trends data, which may serve as a more stable and broadly available measure of public attention than platform-specific sources such as X/Twitter or Facebook.

Restricting the project to the modern theatrical era should:
- reduce structural inconsistencies across time periods
- improve feature availability consistency
- increase the likelihood of identifying meaningful relationships for current-era movies

If the model performs well, I may later expand the timeline to test whether the learned relationships represent more universal “core” drivers of box office performance across eras.

---

### 2. Target Adjustment: Opening Week to Total Gross

Sequels tend to benefit from strong pre-release hype and established audiences, leading to heavily front-loaded opening weekends. However, they also appear to experience steeper declines throughout their theatrical runs compared to original films.  

If opening weekend revenue is used as the target, the `is_sequel` feature may dominate the model and reduce the nuance of the predictions. To better capture longer-term theatrical performance, I am transitioning the prediction target from opening weekend gross to total theatrical gross.

---

### 3. Feature Reduction: Word-of-Mouth

I want the model to focus primarily on features that are within a studio’s control. As a result, I have decided to exclude traditional word-of-mouth (WOM) variables and other forms of audience-generated discourse from the model.  

Instead, I will prioritize features tied to studio-controlled factors such as:
- cast involvement,
- intellectual property (IP),
- marketing-related signals,
- and other studio-generated content where available.

I recognize that excluding WOM will likely reduce predictive performance. However, I accept this tradeoff because the project is intended to evaluate controllable studio decisions rather than uncontrolled public reception. In some cases, factors such as star power or franchise recognition may indirectly serve as proxies for WOM effects.

This creates some tension regarding target selection. Opening weekend gross is less influenced by WOM, making it theoretically attractive. However, the dominance of sequel-driven hype in opening weekend performance makes me hesitant to rely on it as the primary target.

---

### 4. Omitting Sequels from Predictions

Sequels will remain in the dataset for contextual calculations, such as:
- the number of competing films within *n* days of release,
- market saturation,
- and release window dynamics.

However, the model itself will only generate predictions for original films. Predicting sequel performance appears substantially easier because prior installments provide strong reference points, and many core features remain relatively stable across entries in the franchise.

Because sequels are being excluded from the prediction target, opening weekend gross once again becomes a more reasonable target variable.

---

### 5. Domestic Films Only

I will restrict the dataset to domestic U.S. films only. International films may follow substantially different market dynamics, release strategies, audience behaviors, and distribution patterns. Including them could introduce additional noise and reduce the effectiveness of the model.

---

### 6. Kaggle dataset as Box Office filter

The Kaggle box office dataset is used only as a theatrical-release candidate filter. I could've filter the film from IMDB .tsv file by scraping The Number for box office information, but I would take too long. The Kaggle dataset is not treated as the authoritative source for final box office variables. Final opening weekend box office fields are collected separately from The Numbers after filering.
