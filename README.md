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

- **Python** was used to categorize each Facebook post for analysis and create some vizualizations.
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

Upon implementing this methodology, I effectively categorized 80% all Facebook posts in the dataset. The remaining 20% posts which fell in the **Other** category were categorized manually by reviewing each Facebook post and understanding the context.

You can access the Python code used for content categorization & vizualization by clicking [here](https://github.com/akshay-joshi-25/Social-Media-Content-Insights-Analysis-of-CNN-BBC-Al-Jazeera-and-Reuters/blob/main/Categorization%20and%20Vizualization.ipynb)

# 📈 **Content Insights Analysis**

### Facebook Posts by Topic — Al Jazeera, BBC, CNN & Reuters (Jan 1–Mar 15, 2024)

<img width="1271" height="699" alt="image" src="https://github.com/user-attachments/assets/ba8ff0ca-5819-4fb7-862a-3a87bb36e65b" />

**Overall Posting Volume**

* Posting volume is relatively consistent across outlets:

  * **BBC News & Reuters**: ~1,000 posts each
  * **Al Jazeera**: 981 posts
  * **CNN**: 753 posts (lowest, more selective)
* Despite similar output levels, there are **significant differences in how content is distributed across topics**, indicating distinct editorial strategies rather than volume-driven differences.

**Outlet-Level Insights**

**Al Jazeera — Highly conflict-focused**

* **53%** of content dedicated to the **Israel–Palestine conflict**
* By far the **highest single-topic concentration** among all outlets
* Coverage of other geopolitical issues such as the **Russia–Ukraine War** is also present, though significantly smaller in scale (only **7%** of content).
* Demonstrates a **clear editorial priority and thematic focus**, positioning itself strongly around geopolitical conflict coverage, particularly Gaza.

**BBC News — Broad, general-interest strategy**

* Displays one of the widest topic spreads across all outlets.
* **32%** of posts fall under **Arts, Culture & Society**, the second-largest category across all outlets
* This category mostly includes **lifestyle, human interest, entertainment, and UK-focused domestic content**
* Other major categories contributing to 8-10% of total posts are **Crime & Justice (10%)**, **Health & Science (9%)**, **Europe (8%)**, and **Climate & Environment (8%)**. 
* This indicates a strategy focused on **balancing hard news with lighter or culturally relevant content**, rather than specializing in one specific topic like Al Jazeera.

**CNN — Balanced and curated content mix**

* Displays a relatively more **even distribution across topics**, with no single category accounting to more than 25% of the total content volume.
* That said, a stronger emphasis appears in the coverage of **Arts, Culture & Society (22%)**, and **US Politics and Elections (18%)**.
* Other topics like **Health & Science (9%)**, and **Technology (8%)** are given moderate coverage.
* Indicates CNN's content strategy involves **blending US-centric political discourse with socio-culturally engaging content**
* Lower posting volume (**753 posts**) suggests a **more selective, quality-over-quantity approach**

**Reuters — Globally distributed, topic-diverse**

* Coverage is far more more evenly spread across **multiple regions (Europe, Asia, US, etc.) and themes (technology, politics, culture)**
* No single topic accounts to more than 15% of the total coverage, reflecting Reuters’ role as a **global wire service rather than a commentary-driven publisher**.
* Indicates Reuters' content strategy is centered on:
  * neutrality,
  * broad international coverage, and
  * informational balance over emotional intensity

**Israel–Palestine Coverage Comparison**

* **Al Jazeera**: Dominant focus (**53% of posts**)
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
  * Consistently high posting volume (**1K posts**)
* Strong performance across likes, comments, and shares suggests **broad and consistent audience interaction at scale**

**CNN delivers the most engaging content per post (efficiency leader)**

* Records the **highest engagement per post (1.54K)** despite posting less (**753 posts**)
* Particularly strong in **comments**, indicating more discussion-driven or provocative content
* Suggests **higher content quality or relevance per post**, even with a smaller audience than BBC

**Al Jazeera punches above its weight (high relative performance)**

* Generates **1.21M total engagement** with only **14M followers**, far fewer than BBC or CNN
* Maintains solid engagement per post (**1.24K**)
* Indicates **strong audience connection and efficient content strategy relative to its size**

**Reuters underperforms across all metrics**

* Lowest **total engagement (149K)** and **engagement per post (150)** despite posting frequently (**1K posts**)
* Significantly lower likes, comments, and shares suggest **weaker audience resonance or less engaging content format**

**Key takeaway**

* **BBC News dominates in overall reach and total engagement** due to scale
* **CNN leads in content effectiveness**, maximizing engagement per post
* **Al Jazeera performs efficiently relative to its smaller audience**
* **Reuters lags considerably**, indicating an opportunity to improve content strategy or audience engagement approach
* **A larger audience does not guarantee higher content engagement**
  
  * CNN’s engagement per post is **17% higher** than that of BBC News, despite having significantly fewer Facebook followers.
  * Al Jazeera’s engagement per post reaches **94% of BBC News’ level**, despite having only **one-fifth of its Facebook followers**.

### Engagement Score by Topic — Al Jazeera, BBC, CNN & Reuters (Jan 1–Mar 15, 2024)

<img width="1276" height="633" alt="image" src="https://github.com/user-attachments/assets/025db460-29c2-4c06-ba51-bef779f9f665" />

**Al Jazeera — Conflict as the Core Engagement Driver**

* **1.21M total engagement**, heavily concentrated in **Israel–Palestine content**
* Conflict accounts for **74% of total engagement**, vs. 53% of posts
* Indicates **significantly higher engagement per post** for Gaza-related content
* Demonstrates strong alignment between **editorial focus and audience interest**
* Conflict coverage generates **disproportionate emotional reactions**, amplifying engagement

**BBC News — Scale Combined with Cultural Resonance**

* Highest overall engagement: **1.31M**
* **Arts, Culture & Society** remains dominant accounting to **40% of total engagement**, vs. 32% of posts
* **Health & Science** is a distant second accounting to **10% of total engagement**, vs. 9% of posts
* Indicates BBC News’ **lifestyle, entertainment, and human-interest content strategy delivers strong interaction**

**CNN — Entertainment Drives Engagement**

* ~**1.16M total engagement** with a **more balanced posting strategy**
* **Arts, Culture & Society** accounts for **30% of total engagement**, vs. 22% of posts, followed by **US Politics & Elections** which makes up **25% of total engagement** vs. 18% of posts
* Indicates that CNN’s audience is more likely to engage with **entertainment, cultural, and U.S. election–related content** than with war or conflict-related content.

**Reuters — Minimal Engagement Despite High Volume**

* ~**120K total engagement**, vs. ~**1.1M–1.35M** for other outlets
* Posts at a **similar volume (1K posts)** but generates **<10% of peer engagement**
* Indicates a **significant gap between content output and audience interaction**
* Likely because Reuters’ **neutral content and fact-driven reporting style**, is less polarizing and conversley, less engaging on social media
* Suggests Facebook is used primarily as a **distribution channel rather than an engagement platform**

**Key Takeaway**

* **Engagement is driven by topic resonance, not content volume**
* **Al Jazeera** → Leads through conflict-driven engagement
* **BBC** → Wins on scale with strong lifestyle content performance
* **CNN** → Most engagement comes from entertainment, culture, and U.S. election based content
* **Reuters** → Lowest engagement despite similar volume as its content is more neutral and doesn't strike a chord with the masses

**Recommendation**

To shape content strategy and boost engagement, I strongly recommend prioritizing emotionally resonant content over simply increasing posting volume on social media. **Content (Quality) outweighs Volume (Quantity).**




<img width="1000" height="828" alt="image" src="https://github.com/user-attachments/assets/ea09b363-ca1c-4db9-9d88-1acf0d1a8d79" />



