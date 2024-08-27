## Sentiment Analysis of RSS Feed Entries

This script analyzes the sentiment of news entries from an RSS feed using the Hugging Face `heBERT` sentiment analysis model. It extracts the text from each entry in the feed, sends it to the model, and filters out entries with positive sentiment. The sentiment score is converted to a percentage (0-100%) for easier interpretation.

### Features:
- **RSS Feed Parsing**: The script uses the `feedparser` library to parse an RSS feed and extract relevant content (e.g., titles and summaries).
- **Sentiment Analysis**: Each entry is analyzed using the Hugging Face Inference API with the `heBERT` sentiment analysis model.
- **Positive Sentiment Filtering**: Only entries with a positive sentiment are displayed.
- **Score Conversion**: The sentiment score is converted from a 0-1 range to a 0-100% range, providing a more intuitive confidence level for the sentiment.

### Usage:
1. **Set Up the Environment**:
   - Install the required dependencies:
     ```bash
     pip install feedparser requests
     ```

2. **Configure the API**:
   - Replace the placeholder `hf_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx` with your actual Hugging Face API token.

3. **Run the Script**:
   - The script will parse the RSS feed, analyze the sentiment of each entry, and print only the entries with positive sentiment along with their confidence scores.

### Example Output:
```
Text: Example news article title and summary...
Sentiment: Positive (85.00%)
--------------------------------------------------------------------------------
```

This output indicates that the article has a positive sentiment with an 85% confidence level.

### Customization:
- **Feed URL**: You can change the RSS feed URL to analyze a different feed by modifying the `feed_url` variable.
- **Thresholds**: You can adjust the sentiment score threshold or customize the conditions for displaying entries based on your needs.

---

This description provides a clear and concise explanation of the script's functionality, usage, and customization options, making it suitable for inclusion in a README file.# news_positive
this is news classification project which is used to display only positive news and it get input from rss feed
