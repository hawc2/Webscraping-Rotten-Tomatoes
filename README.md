# Scraping TV & Film Reviews

Collecting and analyzing film/TV review data from various sources. Work in progress.

## rotten-tomatoes/

Older notebooks for scraping Rotten Tomatoes critic and user reviews directly. These work but note that RT's Terms of Service prohibit automated scraping — kept here for reference.

## omdb/

Uses the [OMDb API](http://www.omdbapi.com/) (legit, free tier) to pull scores and metadata. Current focus: building a dataset of Trump-related films and documentaries.

- `trump-films-omdb.ipynb` — pulls 21 films from OMDb with IMDb, RT, and Metacritic scores
- `trump-films-omdb.csv` — the raw dataset
- `trump-films-analysis.ipynb` — score analysis + NLP on plot descriptions (VADER sentiment, TF-IDF, word clouds by political perspective)
- `trump-films-analyzed.csv` — enriched dataset with sentiment scores and perspective tags

Early findings: pro-Trump docs get zero RT critic coverage, use more adversarial framing in descriptions ("opposition," "conspiracy," "challenges"), and have the most negative plot description sentiment despite being supportive of their subject.
