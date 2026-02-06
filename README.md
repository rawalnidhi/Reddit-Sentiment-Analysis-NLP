# 🤖 Public Perception, Fairness, and Algorithmic Bias in AI Hiring
**A Data-Driven Study of Ethical Concerns using NLP and Reddit Discourse**

## 📖 Project Overview
[cite_start]This project investigates how the public perceives the integration of Artificial Intelligence (AI) in workplace recruitment and employee evaluation[cite: 1, 6]. [cite_start]By analyzing a dataset of **2,998 Reddit posts**, specifically identifying **729 hiring-related discussions**, the study explores emerging ethical gaps in fairness, transparency, and accountability[cite: 12, 13].

## 🎯 Why This Study? (Research Question)
[cite_start]Organizations increasingly rely on automated résumé screening, algorithmic candidate ranking, and AI-driven interview assessments[cite: 7]. [cite_start]This project asks: **How can organizations ensure fairness, transparency, and accountability when using AI for hiring and employee evaluation?**[cite: 14]. [cite_start]Understanding public sentiment offers critical insight into the ethical gaps that remain unresolved as these systems grow more influential[cite: 15].

## 🛠️ Methodology: How We Did It
[cite_start]The project follows a rigorous Data Science pipeline to extract insights from unstructured social media data[cite: 13]:
* [cite_start]**Data Collection**: 2,998 Reddit posts related to workplace AI were collected and filtered for hiring-specific terms like "hire," "interview," "candidate," and "application"[cite: 57, 58].
* [cite_start]**NLP Preprocessing**: Applied text cleaning through tokenization, punctuation removal, stopword filtering, and lemmatization[cite: 59].
* [cite_start]**Sentiment Analysis**: Computed sentiment scores using **VADER** to categorize discussions into positive, negative, and neutral categories[cite: 61, 62].
* [cite_start]**Thematic Detection**: Used ethical keywords—*bias, fairness, transparency, privacy,* and *accountability*—to identify relevant concerns[cite: 62].
* [cite_start]**Statistical Validation**: Performed a **t-test** to compare average sentiment between hiring and non-hiring discussions to determine distinct emotional tones[cite: 63].
* [cite_start]**Topic Modeling**: Applied **Latent Dirichlet Allocation (LDA)** to uncover thematic differences in user discussions[cite: 268].

## 📊 What We Achieved (Key Results)
* [cite_start]**Transparency as a Priority**: Transparency was identified as the most prevalent ethical concern, followed by fairness and privacy[cite: 173].
* [cite_start]**Emotional Intensity**: Hiring discussions were found to be statistically more personally and emotionally charged compared to general technical AI talk[cite: 276, 286].
* [cite_start]**Negative Sentiment Drivers**: Discussions involving **Accountability** and **Bias** skew more negative, reflecting unresolved harms and skepticism[cite: 194, 284].
* [cite_start]**Thematic Divide**: Topic modeling revealed that hiring posts revolve around personal career transitions and uncertainty, while non-hiring posts remain solution-focused and technical[cite: 269, 272, 287].

---

### Visualizing the Analysis
![Ethical Concerns Mindmap](./images/mindmap.png)  
[cite_start]*Figure 1: Mind map of ethical concerns in AI hiring systems, including fairness, transparency, and accountability[cite: 43].*

![Ethical Keyword Frequency](./images/Ethical_Keyword_Counts.png)  
[cite_start]*Figure 2: Frequency of ethical keywords in hiring-related Reddit posts, showing Transparency as the leading concern[cite: 188].*

![Negative Post Word Cloud](./images/Negative_PostsCloud.png)  
[cite_start]*Figure 3: Common themes in negative hiring posts highlight issues with "models," "managers," and "jobs"[cite: 133, 169].*

![Overall Sentiment Distribution](./images/Sentiment_Distribution.png)  
[cite_start]*Figure 4: Distribution of sentiment across all Reddit posts about AI in the workplace[cite: 88].*

---

## 🚀 Setup & Installation

### 1. Reddit API Credentials
To fetch data, you must have a Reddit developer account:
* Visit [Reddit App Preferences](https://www.reddit.com/prefs/apps).
* Click **"create app"** or **"create another app"**.
* **Name**: `AI_Hiring_Analysis` (or your preferred name).
* **App Type**: Select **script**.
* **Redirect URI**: Use `http://localhost:8080`.
* Click **"create app"** to get your **Client ID** (under the app name) and **Client Secret**.

### 2. Environment Variables
Create a file named `.env` in your root directory. This project uses the `python-dotenv` library to keep your keys safe. Add your credentials like this:
```text
REDDIT_CLIENT_ID=your_client_id_here
REDDIT_CLIENT_SECRET=your_client_secret_here
REDDIT_USER_AGENT=your_app_name_here

### 3. Install Dependencies

Open your terminal in VS Code and run the following command to install the required Python libraries:
pip install -r requirements.txt

### 4. Run the Analysis

. Open the ai_bias.ipynb notebook in VS Code or Jupyter.

. Ensure your kernel is set to your Python environment.

. Execute the cells in order to reproduce the data fetching, cleaning, and visualizations.
