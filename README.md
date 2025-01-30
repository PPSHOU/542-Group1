# 542-Group1

## Code/ideas reuse statements
Replace the 12 file paths with your own.  
Make sure you have installed the pandas and matplotlib packages before running the code on the Jupyter notebook platform.

## Questions
1. **What is the typical structure of conversations between developers and ChatGPT? How many turns does it take on average to reach a conclusion?**
2. **What is the distribution and average of UpvoteCount and Number?**
3. **What are the top 3 most popular languages?**


## Methodology

### **1. Load and Combine Data**
Used Python to load 12 JSON files consisting of discussion and issue data. Combined the data in Jupyter Notebook and loaded it into a DataFrame using pandas. Displayed the basic information of the combined data.

### **2. Traverse Data and Extract Target Fields**
Traversed the combined data to extract target fields and converted them to appropriate data types, such as **Type**, **RepoLanguage**, **Number**, and **UpvoteCount**.For the **Conversations** field, which is in a list structure, extracted the number of elements and recorded it as **Conversations_num**.

### **3. Perform Statistical Analysis and Visualization**
Aggregated the extracted fields into a new DataFrame.  Viewed the distribution of target fields and plotted distribution bar charts. Analyzed the results for meaningful insights.


## Results and Interpretation

### **Issues vs. Discussions**
The total number of issues is **1,750**, which is **seven times** more than the number of discussions (**250**). This indicates that more issues are encountered than discussions during the development of ChatGPT.

### **Conversation Turn Analysis**
Most conversations require **400 to 570 turns** to reach a conclusion and the **average number of turns per conversation** is **4.85**.

### **Upvote Count and Number Distribution**
The **majority of conversations have an UpvoteCount of 0**, with only a small proportion having UpvoteCounts greater than 0 and the **Number** distribution mostly falls between **20 and 122**, while the average is **1,510** due to the influence of outliers.These observations indicate the presence of **outliers** in both "UpvoteCount" and "Number," although the majority of data points remain within normal ranges.

### **Language Popularity**
The top three most popular languages are **Python**, **TypeScript**, and **JavaScript**, which are far more popular than other languages.This suggests that these three languages are particularly suitable and appropriate for ChatGPT development.

