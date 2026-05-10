# Feature Ideas

## Ex Ante Research Paper Analysis

### 1. Prior Genre Experience
- Number of prior films an actor, director, writer, studio, distributor, or other key entity has worked on within the same genre, actor, director, writer, etc...

### 2. Perceived Genre Classification
- Use NLP on reviews to infer the perceived genre of each movie.
- Create a list of genre tags to capture film's nuaced perception.
- Reviews are used only to understand how audiences/critics perceived the movie’s genre, not as a prediction signal.
- This may differ from the reported genre.

### 3. Historical Momentum Features
- Actor, director, writer, studio, distributor, or genre gross revenue acceleration.
- Possible versions:
  - revenue velocity
  - change in revenue velocity
  - rolling historical growth rate

### 4. Descriptive Title Flag
- NLP-based flag indicating whether the movie title clearly describes the genre, premise, or storyline.
- Manual inspection will not be used due to time constraints.

### 5. Descriptive Title × Budget Interaction
- Interaction between the descriptive title flag and production budget.
- Idea: descriptive titles may matter more for lower-budget or under-promoted films.

### 6. Release Timing and Competition Features
- Distance from nearest seasonal demand peak.
- Nearest seasonal demand peak category.
- Number of similar-genre movies released within 20 days.
- Number of general movies released within 20 days.
- Number of similar-genre movies with similar budgets released within 20 days.
- Number of general movies with similar budgets released within 20 days.
- Budget × distance from nearest seasonal peak interaction.

### 7. Local Genre Environment
- Mode genre among movies released within 60 days of the target movie.

### 8. Recency Features
- Days since actor’s last movie release.
- Days since director’s last movie release.
- Days since IP/franchise’s last movie release.


## Ex Post Research Paper Analysis

### 1. Audience Perceived Genre Entropy

- Measure disagreement or dispersion in how audiences describe the movie’s genre using review and discussion text rather than official studio labels.

### 2. Pre-Release Attention and Awareness Signals

- Google Trends activity for actors, directors, franchises/IP, and film titles leading up to release.
- Actor/director x film titles Google Trends activity leading up to release

### 3. Relative Market Positioning Features

- Budget relative to nearby competing releases, franchise saturation within the release window, and similarity density among neighboring films.

### 4. Plot Description Sentiment and Sentiment Entropy
