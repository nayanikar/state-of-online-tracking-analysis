# Introduction
- Have you ever seen yourself surfing Amazon for headphones, and now every page you visit offers advertisements for headphones
- Nowadays, trackers are incorporated on websites. These trackers collect data under the pretense of improving the user experience. They are, however, used to profile a user's attributes and behaviors by analyzing location history, browsing history, and other data to deduce your gender, ethnicity, interests, and habits.
- This online profile is then used for targeted advertising.
- In this poster, we have tried to decode these trackers' usage, the websites that use them, and the organization that operates them.
- Policymakers can use this study to design laws for online tracking. Another application could be to develop sophisticated tracker blockers.

# Data
- The data for this study is self collected using the DuckDuckGo Privacy Essentials Chrome Extension, and [DuckDuckGo Tracking Radar](https://github.com/duckduckgo/tracker-radar).
- A final copy of the data can be found [here](https://www.kaggle.com/datasets/kaustubhlohani/trackers-on-popular-websites-105-countries?datasetId=3260291&sortBy=dateRun&tab=profile)


# Data Collection
## Web Scraping:
- A list of popular websites was compiled using Kaggle.
- Further a Python program was built using the pyautogui package, to automate the collection of html for the blocked trackers sections from websites  using the DuckDuckGo extension.
- Using the beautiful soup library in python the collected html files were parsed for the tracker data and saved in a csv file.
- Finally, a script was written for preliminary cleaning of the collected data.
## Data Preprocessing:
- Using pandas library in python the scraped data was cleaned, and additional columns were added.
## Collecting data related to organizations that owns & operates the trackers:
- First, the preprocessed data was grouped on tracker URL. 
- A Python script was then used to search for the tracker URLs in the DuckDuckGo Tracker Radar data. The script extracted information about the owners of each tracker, was then combined with the existing data.

# Results
See [Poster.pdf](https://github.com/k-lohani/state-of-online-tracking/blob/main/Poster.pdf) for results.

# Conclusion and Future Work
- Among the 585 websites from 105 countries, only 104 websites – 17.8% had no embedded trackers.
- Legislations such as GDPR & CCPA (California Consumer Privacy Act) require websites & associated third parties to get consent before collecting and processing personal data. However, a [study](https://arxiv.org/abs/2202.00885) found that user data is collected and processed even after users opt out.
- Therefore, using a tracker blocker such as DuckDuckGo or browsers such as Mozilla and Safari, which have tracker blockers baked into them, is the user’s best bet to be safeguard their data against the trackers.
- This study is currently done on a limited number of popular websites (585) for each country (105 – countries) and can be expanded further by increasing the number of websites analyzed.
- Data collected by the trackers should also be looked at to analyze its impact on influencing users’ choices.
# state-of-online-tracking-analysis
