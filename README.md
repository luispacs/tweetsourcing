# TweetSourcing: Finding sources behind tweets you see.
This python program is intended as a tool to make fact checking easier. 
Information spreads faster than ever due to social media and proliferation
of the internet. Not everyone is going to fact check before they post so it is 
on the individual to be skeptical and perform due diligence.<br>

## What this program does do:
- Takes a tweet URL and extracts the text/image content.
- Performs a reverse google image search for the image to see where else it has been used.
- Extracts keywords from the text and searches from news sites with varying political biases for articles about the topics.

## What this program <b>does not</b> do:
- Search for video sources.
- Tell you whether the tweet's statements are true. This is simply a tool to help you draw your own conclusions.

### Ways this can be improved:
- Improve tweet keyword recognition with custom nltk model, custom stop words, etc.
- Add backup search api for when the google api reaches its limit. (Bing api?)
    - Currently only keyword compares the first 50 google results as a method to allow for more searches per day.
- Implement as a web app.
- Speed up categorize_news() function.