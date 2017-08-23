The goal of this project was to distill topics from press briefing topics and visualize how they ebbed and flowed over time. The resulting timelines reflect administration priorities as well as external events that came to dominate the narrative. I scraped all the press briefings from the Obama years from the whitehouse.gov archives and used natural language processing to perform the topic modeling.

<p align="center"><strong>Visualizing the rise of ISIS</strong></br>
<img src="https://github.com/ejm714/press_briefing_topic_timelines/blob/master/topic_timeline_isis.png?raw=true" alt="Topic timeline: ISIS" width="700">
</p>

**Languages**: Python  
**Libraries**: nltk, sklearn, gensim, spacy, plotly, BeautifulSoup  
**Methods**: Natural language processing (TFIDF, SVD), clustering  

Replication notes:

- fletcher_scraping scrapes press briefings from the Obama years
- fletcher_analysis_limited_data tries different ways of topic modeling on a subset of the data (5000 documents)
- fletcher_full_data_lsa_kmeans_80_clusters runs an LSI with 200 dimensions and kmeans with 80 clusters on the full dataset (Obama's second term, ~125,000 documents)
- plotly_80_clusters plots the topics over time in plotly
- fletcher_presentation_EM includes my slides

The interactive visualization of topic timelines is available here: https://plot.ly/~ejm714/25.embed
