# Understanding Tornado Impacts Through Facebook Conversations: A Longitudinal Study Using LLMs 
The tornado outbreak in the US in 2011 was one of the worst natural disasters in recent history. It left a big mark on communities and sparked a lot of conversation on social media. Based on Facebook posts made during the timeline of the disaster, this thesis presents a new dataset that shows the timeline and posts of public sentiment and behavioral at during this important event. The main goal is to look at how people's feelings and actions changed during the tornado outbreak. It will give us a full picture of how user opinion changes in real time. 
Large language models (LLMs) like GPT, BERT and twitter-sentiment-pl are used in the study, along with more advanced methods. I used topic modeling and hybrid mood analysis.
The study includes a **comparison of LLMs**, checking how well each model works on the **brand-new dataset**. **I fine-tuned the LLMs from their basic model according to my database**. So that it can predict more accurate sentiment of the Facebook posts. It shows a way to do sentiment analysis in real time so that we can use the technique to prepare a better and quicker disaster management system. This has important effects for emergency response plans and planning for real-time crisis communication.

The development of LLMs like **BERT, GPT-3, and DeBERTa** marked a transformative change in sentiment analysis. These models use contextual embeddings to deal with tricky language features like sarcasm, hidden meaning, and long-lasting relationships. For example, DeBERTa's "disentangled attention" system picks up on subtle semantic connections, which makes it great for analyzing opinions on social media. This Research highlights their value in assessing public sentiment during natural disasters and health emergencies.

**Database Overview**
Natural disasters have a huge effect on communities, making it hard to live and communicate. One powerful example is the tornado that hit Tuscaloosa, Alabama, on April 27, 2011. To analyse sentiment and behavioural shifts of a tornado event, a database of approximately 23,000 Facebook posts from 4,000 individuals was created for this study. The data was classified into three unique phases: before, during, and after tornado offering a longitudinal perspective on emotional and thematic trends.
This database serves two main purposes. One is to assess human perceptions and responses to natural disasters through sentiment analysis, and the second one is to evaluate the feasibility of employing social media for real-time crisis management. This strategy aligns with other research emphasizing the necessity of systematically curated social media data for understanding public opinion during critical events.

**Large Language Models (LLMs)**
Large Language Models (LLMs) have transformed **natural language processing (NLP)** by facilitating context-sensitive, high-precision text analysis. For example, ChatGPT is a useful tool for evaluating the complex and emotionally charged language frequently found in social media messages because of its proficiency in sentiment classification, contextual understanding, and summarization.
**BERT-based models** excel in aspect-based sentiment analysis (ABSA). It can effectively extract sentiments on certain subjects and entities. It has been shown that integrating contextual embeddings (such as those from BERT) with sentiment analysis tasks greatly enhances performance, particularly when resources are limited. (6)
The ability of LLMs to analyze complicated datasets like Facebook posts is further increased by their hybridization with other NLP approaches like topic modeling and coreference resolution.

**Methodology:**
![Roadmap](https://github.com/user-attachments/assets/56bfde72-3c64-4e52-99cb-493942318a14)

 I started with raw Facebook data. Then, I scrapped that and collected the texts and other entities in a database. I then leveled the data with OpenAI. After that I trained LLM models with a part of data. Observing that result I fine-tuned the LLM model and ran the rest of the data. That is how I could get a sentiment score for each post.

Data Preprocessing: 
Step 1 was data preprocessing. I had the Facebook post of 4000 people in text format. Then, I scrapped, organized and stored those posts with the help of **Pandas and sql**.   Following this, I processed all of the posts and organized them into an Excel file. I organized almost 23000 posts including participant numbers. I also stored other entities.(Likes, shares, replies). I converted the text file of every participant and stored it in Excel. The code file of this process 'Data_Extraction_p1'. Then I combined the extracted posts of every applicant and combined those to build a database. 
Leveling and scoring data: I scored the Facebook post into three criteria. (Positive, Neutral, Negative). In Step 2, I leveled and scored the sentiments of all 23000+ Facebook posts with GPT4 and openAI. It gave me great results. The code file is: Sentiment-Analysis (OpenAi).A part of the output data can be found as 'processed_sentiments_OpenAI'. Here is an example. 
![ex sentiment openai](https://github.com/user-attachments/assets/7de3aa87-2092-4d63-8053-361a583eb64a)


