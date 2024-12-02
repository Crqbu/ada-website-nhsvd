---
layout: default
title: Home
---


# Who Dies the Most? The Tragic Truth About Movie Mortality

## Introduction: Setting the Scene

Imagine this: the final showdown between the hero and the villain. The stakes are high, and the question looms—*Who will make it out alive?* Movies have always drawn us into tales of triumph and tragedy, but have you ever wondered if certain characters are doomed from the start? Why do mentors so often sacrifice themselves? Why do villains almost always meet their demise? And most importantly, is Sean Bean truly the king of cinematic deaths?

In this data story, we dive into the CMU Movie Summary Corpus and use machine learning to uncover who dies the most, why, and how these patterns differ across genres and tropes. Let’s uncover the hidden patterns of on-screen mortality.

---

## 1. The Data: Behind the Scenes

To uncover movie mortality secrets, we used a rich dataset containing:
- **Movie Metadata**: Information on thousands of films, including genres and release dates.
- **Character Metadata**: Details about hundreds of thousands of characters, including their associated actors.
- **Plot Summaries**: Textual descriptions that hold clues about character fates.

We combined these datasets to extract death-related insights. Using text mining, we identified characters mentioned as dying in plot summaries. By clustering characters into tropes like "villains" and "heroes," we created a "mortality index" to quantify the likelihood of death across different roles and genres.

---

## 2. Text Mining: Detecting Deaths in the Wild

Our first challenge was finding death mentions in plot summaries. Armed with a comprehensive list of death-related keywords (e.g., *"killed," "dies," "murdered"*), we scanned over 40,000 movie summaries for evidence of character mortality. Here’s what we found:

- **50.7% of movies contain character deaths.**
- **Top Death Genres**: Horror, Action, and War films take the lead in character casualties.
- **False Positives**: Sometimes our model misclassified phrases like *"nearly kills Batman"* as actual deaths. This inspired us to refine our methods further.

![Genre-specific mortality rates](link_to_your_genre_mortality_visualization)

---

## 3. Tropes and Clusters: Who’s the Most Doomed?

Next, we grouped characters into tropes such as:
- **"Mentors"**: Wise characters who guide the hero but often sacrifice themselves.
- **"Villains"**: Always plotting, rarely surviving.
- **"Heroes"**: Sometimes they fall, but their survival is more likely.

Using embeddings and KMeans clustering, we identified patterns in these tropes. Here’s what stood out:
- **Mentors have the highest mortality rate** (65%), often dying to inspire the hero.
- **Villains follow closely at 60%.** Their deaths serve justice and satisfy audience expectations.
- **Comedic sidekicks rarely die, with a survival rate of over 80%.**

![Character Tropes Embedding Visualization](link_to_your_tropes_visualization)

---

## 4. Actors with a Death Wish

Some actors just can’t seem to catch a break. Analyzing death frequencies in their roles, we found:
- **Sean Bean** is confirmed as Hollywood's most unlucky actor, with 72% of his characters meeting their demise.
- Other high-mortality actors include Gary Oldman and Leonardo DiCaprio.

Meanwhile, comedic actors like Jim Carrey and Adam Sandler rarely take on roles that involve death.

![Actor Mortality Leaderboard](link_to_your_actor_mortality_visualization)

---

## Conclusion: What We Learned

This data story has uncovered fascinating truths about movie mortality:
- **Mentors and villains are the most doomed.**
- **Comedic characters and heroes are most likely to survive.**
- **Sean Bean remains the undisputed champion of cinematic deaths.**

By blending text mining, machine learning, and data visualization, we’ve turned the tragic into the intriguing. So next time you watch a movie, ask yourself—*Who’s most likely to die?* The answer might just surprise you.

---

### Explore More
Curious about your favorite character? Explore our [interactive visualization](link_to_visualizations) or dive into the [full analysis on GitHub](link_to_repo).
