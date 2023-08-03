# Text-Analysis-On-TED-Talks
Title: Analysis of TED Talks by Speaker David Hanson and Speaker Chris Burkard

Introduction:
This report analyzes two TED Talks delivered by speakers David Hanson and Chris Burkard. David Hanson, a roboticist, explores the creation of human-like robots capable of showing emotions, while Chris Burkard, a photographer, shares his experiences capturing stunning photographs of nature in remote places. The analysis aims to identify common themes, topics covered, and compare their presentation styles.

Methods:
The analysis follows several steps, starting with data collection from the "DsEssex" package. If the package is not already installed, the code in the report will automatically install it using the "drat" package. The "dsEssex" package is added as a repository using "drat::addRepo()" and then installed using "install.packages()". Once the package is installed, text preprocessing involves removing stopwords and tokenization using the "tidytext" package. The report employs text analysis to gain insights and patterns, including sentiment analysis to understand the speakers' emotional tone. Visualization is done using "ggplot2," "Cowplot," "ggthemes," and "ggrepel" packages.

install the package if it hasn't been already installed
if(!require(dsEssex)){
  install.packages("drat")
  drat::addRepo("statcourses")
  install.packages("dsEssex")
}

Results:
Data preprocessing reveals that both speakers intentionally avoid repeating words frequently, engaging the audience with a diverse vocabulary. David emphasizes "robots," reflecting his expertise, while Chris frequently uses "just," possibly downplaying the difficulty of his work.

Text analysis visualizations show the top 15 words used by each speaker, shedding light on their interests and communication styles. Sentiment analysis indicates that both speakers emphasize positive sentiments such as "favorite" and "great," while David focuses on empathy and intelligence, and Chris mentions "cold" and "joy."

Conclusion:
Chris Burkard's TED Talk on "The joy of surfing in ice-cold water" evokes a balanced sentiment with an overall positive score. While their topics differ significantly, both speakers share a passion for exploring possibilities in their respective fields. The talks highlight the intersection of technology and nature, emphasizing the potential benefits that can arise from such interactions.

Overall, this analysis provides valuable insights into the talks of David Hanson and Chris Burkard, shedding light on their communication strategies and the reception of their ideas by the audience. The report ensures the availability of the "dsEssex" package by automatically installing it if not already present in the R environment, making it easier for others to reproduce and extend the analysis.

