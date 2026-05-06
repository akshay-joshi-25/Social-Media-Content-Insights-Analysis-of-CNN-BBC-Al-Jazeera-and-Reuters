# 📊 Facebook Content Insights Analysis of Leading News Channels

The objective of this project is to analyze and compare the content strategies of Al Jazeera, BBC News, CNN, and Reuters, in order to identify which types of content drive the highest engagement and uncover actionable insights for optimizing news content performance.

# 📌 **Overview**

This project will cover the following:
1. Conduct a high-level analysis of the type of content posted by Al Jazeera, BBC News, CNN, and Reuters.
2. Identify top performing content cohorts in terms of overall engagement for Al Jazeera, BBC News, CNN, and Reuters.

# 📂 **Datasets**

The dataset used for this project was publicly made available on Kaggle. Based on the description, it was curated by collecting publicly available engagement data (likes, comments, shares) from Facebook posts of official accounts of Al Jazeera, BBC News, CNN, and Reuters, using ethical scraping or aggregation methods rather than an official API.

You can access the dataset by clicking [here](https://www.kaggle.com/datasets/kanchana1990/global-news-engagement-on-social-media?select=bbc.csv)

# 🔧 **Tools Used**

- **Python** was used to categorize each Facebook post for analysis.
- **Excel** was used for data visualization and exploratory data analysis.

# 🧾 **Categorization of the Dataset**

The dataset used for this project originally contained only four columns:
- **text** - Title of the Facebook post.
- **likes** - Number of people who liked the Facebook post.
- **comments** - Number of comments on the Facebook post.
- **shares** - Number of times the Facebook post was shared.

Because the dataset did not contain any categorical variables, any kind of cohort analysis or content insights analysis was impossible. To address this issue, I wrote a Python code to create another column that categorized each Facebook post based on the keywords present in the title of the post. For instance, Facebook posts containing words such as:
- *'Israel', 'Palestine', 'Gaza'*, etc. were categorized as **Israel-Palestine Conflict** posts.
- *'Russia', 'Ukraine', 'Putin'*, etc. were categorized as **Russia-Ukraine War** posts.
- *'Trump', 'Biden', 'US Election'*, etc. were categorized as **US Politics and Elections** posts.
- *'Oscar', 'Grammy', 'BAFTA'*, etc. were categorized as **Arts, Culture & Society** posts.
- *'Cricket', 'Football', 'Olympics'*, etc. were categorized as **Sports** posts.
- *'Climate', 'Emissions', 'Global Warming'*, etc. were categorized as **Climate & Environment** posts.
- *'COVID', 'Pandemic', 'Vaccine'*, etc. were categorized as **Health** posts.
- *'AI', 'Machine Learning', 'Robot'*, etc. were categorized as **Technology** posts.
- *'Iran', 'Iraq', 'Saudi'*, etc. were categorized as **Middle East & North Africa** posts.
- *'Nigeria', 'Kenya', 'Ethiopia'*, etc. were categorized as **Africa** posts.
- *'Brazil', 'Mexico', 'Venezuela'*, etc. were categorized as **Latin America** posts.
- *'EU', 'Germany', 'France'*, etc. were categorized as **Europe** posts.
- *'India', 'China', 'Australia'*, etc. were categorized as **Asia & Pacific** posts.
- *'Human Rights', 'Discrimination'*, 'LGBTQ', etc. were categorized as **Human Rights & Social Issues** posts.
- *'Economy', 'GDP', 'Investment'*, etc. were categorized as **Economy & Business** posts.
- *'Humanitarian', 'Famine', 'WFP'*, etc. were categorized as **Humanitarian Crisis & Aid** posts.
- *'Verdict', 'Guilty', 'Police'*, etc. were categorized as **Crime & Justice** posts.
- The rest were categorized as **Other** posts.

Upon implementing this methodology, I effectively segregated all Facebook posts of Al Jazeera, CNN, BBC News, and Reuters into 18 different categories.

# 📈 **Content Insights Analysis**

### Facebook Posts by Topic — Al Jazeera, BBC, CNN & Reuters (Jan 1–Mar 15, 2024)

<img width="1271" height="699" alt="image" src="https://github.com/user-attachments/assets/dddefba5-1439-4655-b6c9-e3c398341525" />

**Overall Posting Volume**

* Posting volume is relatively consistent across outlets:

  * **BBC News & Reuters**: ~1,000 posts each
  * **Al Jazeera**: 981 posts
  * **CNN**: 753 posts (lowest, more selective)
* Despite similar output levels, there are **significant differences in how content is distributed across topics**, indicating distinct editorial strategies rather than volume-driven differences.

**Outlet-Level Insights**

**Al Jazeera — Highly conflict-focused**

* ~**52–55%** of content dedicated to the **Israel–Palestine conflict**
* By far the **highest single-topic concentration** among all outlets
* Demonstrates a **clear editorial priority and thematic focus**, positioning itself strongly around geopolitical conflict coverage, particularly Gaza.

**BBC News — Broad, general-interest strategy**

* ~**55–60%** of posts fall under **“Other”**, the largest category across all outlets
* Likely includes **lifestyle, human interest, entertainment, and UK-focused domestic content**
* Indicates a strategy focused on **maximizing mass engagement and accessibility**, rather than specializing in hard news topics
* Additional presence in **Arts, Culture & Society** reinforces this pattern

**CNN — Balanced and curated content mix**

* Displays the **most even distribution across topics**, with no single dominant category
* Covers a mix of **US politics, international conflicts, and arts/culture**
* Lower posting volume (**753 posts**) suggests a **more selective, quality-over-quantity approach**
* Strong engagement in commentary-heavy areas (e.g., politics) aligns with its audience profile

**Reuters — Globally distributed, topic-diverse**

* Coverage spread across **multiple regions (Europe, Asia, US, etc.) and themes (technology, politics, culture)**
* Less emphasis on any single topic, including Israel–Palestine
* Reflects its role as a **neutral, global wire service**, prioritizing **breadth and geographic balance** over depth in any one issue

**Israel–Palestine Coverage Comparison**

* **Al Jazeera**: Dominant focus (**>50% of posts**)
* **CNN & Reuters**: Moderate, proportionate coverage
* **BBC News**: Relatively minimal emphasis
* This contrast highlights **fundamentally different editorial priorities**, from conflict-centric to broadly diversified strategies

**Key Takeaway**

* While posting volume is similar, **content strategy and editorial focus vary significantly**:

  * **Al Jazeera** → Deep, conflict-driven coverage
  * **BBC News** → Broad, lifestyle and general-interest content
  * **CNN** → Balanced, curated mix with US emphasis
  * **Reuters** → Globally diverse, multi-topic reporting
* These differences reflect **distinct audience targeting, editorial identity, and positioning on social media**

### Facebook Content Performance by Channel — Al Jazeera, BBC, CNN & Reuters (Jan 1–Mar 15, 2024).

Note: While the original dataset provided data on the number of likes, comments, and shares each Facebook post received, not all interactions are equal.
- **Likes** indicate a relatively low-effort approval.
- **Comments** suggest a deeper interest or emotional response.
- **Shares** reflect a high engagement value as people are not only endorsing the content but also disseminating it.

Therefore, instead of relying on just one of the above metrics for Content Insights Analytics, I created a new metric called **Engagement Score** and used it as the North Star Metric of my analysis.

**Engagement Score** = Likes + (Comments x 1.5) + (Shares x 2)

<img width="1110" height="275" alt="image" src="https://github.com/user-attachments/assets/b36f7ea5-0cbb-4964-bd0a-b633c5515291" />

The above table compares Facebook performance across four news outlets using total engagement and engagement per post.

**Key insights**

**BBC News leads in total engagement (scale advantage)**

* Achieves the **highest engagement score (1.31M)**, driven by:

  * The **largest follower base (61M)**
  * Consistently high posting volume (**1,000 posts**)
* Strong performance across likes, comments, and shares suggests **broad and consistent audience interaction at scale**

**CNN delivers the most engaging content per post (efficiency leader)**

* Records the **highest engagement per post (1,535)** despite posting less (**753 posts**)
* Particularly strong in **comments**, indicating more discussion-driven or provocative content
* Suggests **higher content quality or relevance per post**, even with a smaller audience than BBC

**Al Jazeera punches above its weight (high relative performance)**

* Generates **1.21M total engagement** with only **14M followers**, far fewer than BBC or CNN
* Maintains solid engagement per post (**1,235**)
* Indicates **strong audience connection and efficient content strategy relative to its size**

**Reuters underperforms across all metrics**

* Lowest **total engagement (149K)** and **engagement per post (150)** despite posting frequently (**1,000 posts**)
* Significantly lower likes, comments, and shares suggest **weaker audience resonance or less engaging content format**

**Key takeaway**

* **BBC News dominates in overall reach and total engagement** due to scale
* **CNN leads in content effectiveness**, maximizing engagement per post
* **Al Jazeera performs efficiently relative to its smaller audience**
* **Reuters lags considerably**, indicating an opportunity to improve content strategy or audience engagement approach

