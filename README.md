# 542-Group1      

## Code/ideas reuse statements     
Replace the 12 file paths with your own.       
Make sure you have installed the pandas, numpy, re, sklearn, altair and matplotlib packages before running the code on the Jupyter notebook platform.     

## Summary     
This project presents an in-depth analysis of developer interactions with ChatGPT, focusing on conversation structure, engagement metrics, and language usage trends. By loading and combining data from 12 JSON files, we systematically explored key fields such as conversation counts, upvotes, and programming language preferences. Statistical analysis and visualization techniques were employed to identify patterns and derive meaningful insights.     

## Structure:     
project-root/     
│     
├── project_code1.ipynb              # Notebook covering general analysis or initial exploration     
│     
├── project_code2_Q2.ipynb           # Question 2:Identify patterns in the prompts developers use     
│     
├── project_code3_Q7 explore.ipynb   # Analysis to Question 7:Predict the length of a conversation     
│     
├── report.pdf                       # Final project report in PDF format     
│     
└── README.md                        # Project overview and instructions     

## More about the files:     

#### project_code1.ipynb        
The findings revealed that conversations typically require 400 to 570 turns to reach a meaningful conclusion, with an average of 4.85 turns per conversation, indicating efficient discussion handling. Analysis of engagement metrics showed that most conversations have an UpvoteCount of 0, with occasional outliers receiving significantly higher upvotes. The distribution of the "Number" field predominantly fell between 20 and 122, though outliers raised the average to 1,510.       
Language analysis highlighted Python, TypeScript, and JavaScript as the most popular programming languages, reflecting their versatility and strong ecosystem support for machine learning, server-side logic, and web development. These insights offer valuable perspectives for improving ChatGPT interactions and understanding developer preferences.     

#### project_code2_Q2.ipynb      
Key Features     
Data Extraction: Combines multiple JSON files containing discussion and issue data.     
Feature Engineering:     
Extracts prompt lengths, first words, and response lengths.     
Analyzes keyword patterns using TF-IDF (Term Frequency-Inverse Document Frequency).     
Visualization:     
Bar charts for top starting words in prompts.     
TF-IDF analysis for identifying high-priority keywords.     
State distributions based on selected keywords.     
Insights:     
Common prompt patterns include question-based queries ("how," "what," "can") and technical topics (e.g., "code," "data," "error").     
No significant correlation was found between prompt patterns and issue resolution success.     

#### project_code3_Q7 explore.ipynb     
Key Features     
Data Processing:     
Merges multiple JSON files containing developer discussions and issue data.
Extracts relevant features such as prompt token count, answer token count, keyword usage, and programming language preferences.     
Feature Analysis:     
Identifies common keywords in developer prompts using regex and tokenization.     
Analyzes the distribution of prompts and answers across programming languages.     
Machine Learning:     
Implements K-Nearest Neighbors regression for predicting answer token counts.     

Prediction Accuracy: The KNN model achieved an R² score of 0.9157 and a prediction accuracy of 84.18%.