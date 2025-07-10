# SINNERS-
Analyzing Audience Sentiment Around Ryan Coogler’s Sinners
Overview: I created a multi-source sentiment analysis pipeline for the 2025 film Sinners by Ryan Coogler. The goal was to understand how audiences reacted to the film’s core themes: race, music, and religion — topics that are emotionally and socially resonant.

Data Collection: I collected over 250 audience responses from Reddit and YouTube, focusing on user comments under movie trailers, discussion threads, and early reviews. These platforms were chosen because they offer raw, authentic audience perspectives — unlike curated critic reviews.

Theme & Sentiment Modeling: Using custom keyword matching and TextBlob for sentiment scoring, I built a lightweight NLP pipeline to tag each comment with relevant themes and calculate a sentiment score. I then grouped scores into three categories:
* Positive
* Neutral
* Negative
This allowed me to not only understand how people felt, but also what they were reacting to.

Insights:
* 🔥 Race-related comments skewed more emotionally polarized, showing both strong praise and criticism.
* 🎵 Music comments were overwhelmingly positive — reflecting appreciation for the film’s gospel/hip-hop blend.
* ✝️ Religion-tagged content was mixed, with nuanced sentiments ranging from inspiration to discomfort.
I visualized these findings with bar charts and theme breakdowns using Python’s matplotlib and seaborn.

Challenges & Trade-Offs:
* Reddit API rate limits required batching.
* TextBlob provided simple sentiment scores, but lacked nuance — future versions could use a transformer like DistilBERT for improved accuracy.

Next Steps: I plan to turn this into an interactive Streamlit dashboard where users can filter sentiment by theme, platform, or time.

Tools Used:
* Python, Pandas, Matplotlib, Seaborn
* Reddit API (PRAW), YouTube Data API
* TextBlob for NLP
