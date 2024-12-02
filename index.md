---
layout: default
title: Home
---

# Who Dies the Most? The Tragic Truth About Movie Mortality

## Introduction: Setting the Scene

Imagine this: the final showdown between the hero and the villain. The stakes are high, and the question looms—*Who will make it out alive?* Movies have always drawn us into tales of triumph and tragedy, but have you ever wondered if some characters are doomed from the start? Why do mentors often sacrifice themselves? Why do villains almost always meet their demise? And most importantly, is Sean Bean truly the king of cinematic deaths?

In this data story, we dive into the **CMU Movie Summary Corpus** and use machine learning to uncover the trends in character mortality: *who dies, why, and how these patterns differ across genres and tropes*. Let’s uncover the hidden patterns of on-screen mortality.

---

## 1. The Data: Behind the Scenes

To uncover movie mortality secrets, we used a rich dataset containing:
- **Movie Metadata**: Information on thousands of films, including genres and release dates.
- **Character Metadata**: Details about hundreds of thousands of characters, including their associated actors.
- **Plot Summaries**: Textual descriptions that hold clues about character fates.

We combined these datasets to extract death-related insights. Using text mining techniques, we identified characters mentioned as dying in plot summaries. By clustering characters into tropes like *"villains"* and *"heroes"*, we created a **mortality index** to quantify the likelihood of death across different roles and genres.

---

## 2. Text Mining: Detecting Deaths in the Wild

Our first challenge was finding death mentions in plot summaries. Armed with a comprehensive list of death-related keywords (e.g., *"killed," "dies," "murdered"*), we scanned over **40,000 movie summaries** for evidence of character mortality. Here’s what we found:

- **50.7% of movies contain character deaths.**
- **Top Death Genres**: Horror, Action, and War films dominate the leaderboard in terms of character casualties.
- **False Positives**: Sometimes, our model misclassified phrases like *"nearly kills Batman"* as actual deaths. This inspired us to refine our methods further.

### Visualization: Death Trends by Genre
![Genre-specific mortality rates](images/distribution_of_death_rates_across_movies.png)

---

## 3. Tropes and Clusters: Who’s the Most Doomed?

Characters in movies can often be categorized into recurring archetypes or *tropes*—mentors, villains, heroes, and sidekicks. We analyzed how these character types fared in terms of mortality. Using embeddings and KMeans clustering, we identified patterns in their fates. Here’s what stood out:

- **Mentors have the highest mortality rate** (65%), often dying to inspire the hero.
- **Villains follow closely at 60%**, serving as a cautionary tale or poetic justice.
- **Comedic sidekicks** rarely die, with a survival rate of over 80%.

### Visualization: Tropes in the Semantic Space
Using dimensionality reduction (PCA), we visualized how characters clustered based on their tropes.

![Character Tropes Embedding Visualization](images/embedding_visualization_with_tropes.png)

---

## 4. Actors with a Death Wish

Some actors just can’t seem to catch a break. Analyzing death frequencies in their roles, we confirmed a widely-believed Hollywood trope:

- **Sean Bean** is the undisputed king of cinematic deaths, with **72%** of his characters meeting their demise.
- Other high-mortality actors include **Gary Oldman** and **Leonardo DiCaprio**.
- Meanwhile, comedic actors like **Jim Carrey** and **Adam Sandler** rarely take on roles that involve death, boasting much lower mortality rates.

### Visualization: Actor Mortality Leaderboard
![Actor Mortality Leaderboard](images/actor_mortality_leaderboard.png)

---

## Conclusion: What We Learned

This data story has revealed fascinating truths about movie mortality:
- **Mentors and villains** are the most doomed, while comedic sidekicks and heroes are the most likely to survive.
- **Horror and War genres** are the deadliest, while Comedy is a safe haven.
- **Sean Bean remains the reigning champion of cinematic deaths**, but we now have data to back it up.

By blending text mining, machine learning, and data visualization, we’ve turned the tragic into the intriguing. Next time you watch a movie, ask yourself—*Who’s most likely to die?* The answer might just surprise you.

---

### Curious to Learn More?

Explore our full analysis and code on [GitHub](https://github.com/epfl-ada/ada-2024-project-nhsvd). Dive deeper into the world of movie mortality!

