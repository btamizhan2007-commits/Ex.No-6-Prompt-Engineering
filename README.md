Ex.No.6 Development of Python Code Compatible with Multiple AI Tools

Aim: 

Write and implement Python code that integrates with multiple AI tools to automate the task of interacting with APIs, comparing outputs, and generating actionable insights with Multiple AI Tools.

Explanation:

Develop a python code that integrates multiple AI tool by interacting with their APIs.
Compare outputs from different APIs.
Analyze the response and the Output.

The aim is to understand how to request help from AI tools for tasks like writing Python code, integrating with APIs, comparing outputs, and generating actionable insights.
program:
```
[10:08 am, 26/03/2026] Kavi  (AI DS) : POSITIVE ANALYSIS
from nltk.sentiment import SentimentIntensityAnalyzer
import nltk
nltk.download('vader_lexicon')
generated_text = "This smartphone offers outstanding battery life and an intelligent AI camera that captures stunning photos. i want this into negative statement"

print("Generated Review:\n")
print(generated_text)
sia = SentimentIntensityAnalyzer()
sentiment = sia.polarity_scores(generated_text)
print("\nSentiment Analysis:")
print(sentiment)
if sentiment['compound'] > 0:
    print("\nInsight: The review is positive and suitable for marketing promotion.")
else:
    print("\nInsight: The review tone is neutral or negative.")
[10:08 am, 26/03/2026] Kavi  (AI DS) : NEGATIVE ANALYSIS 

from nltk.sentiment import SentimentIntensityAnalyzer
import nltk

nltk.download('vader_lexicon')


generated_text = "This smartphone does not offer outstanding battery life and does not have an intelligent AI camera that captures stunning photos."

print("Generated Review:\n")
print(generated_text)


sia = SentimentIntensityAnalyzer()
sentiment = sia.polarity_scores(generated_text)

print("\nSentiment Analysis:")
print(sentiment)

if sentiment['compound'] > 0:
    print("\nInsight: The review is positive and suitable for marketing promotion.")
else:
    print("\nInsight: The review tone is neutral or negative.")

Result:
![WhatsApp Image 2026-03-26 at 10 20 45 AM](https://github.com/user-attachments/assets/6783919f-b698-4e3d-a458-5ac1e86d038f)

