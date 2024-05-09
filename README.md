### Dual Subreddit Analysis: A comparative study of Rutgers and UPenn online communities 

#### Project Overview
This project, titled "Dual Subreddit Analysis: A Comparative Study of Rutgers and UPenn Online Communities," leverages advanced machine learning (ML) and natural language processing (NLP) techniques to analyze discussions on the Rutgers and UPenn Reddit subreddits. By examining posts from these subreddits, we aim to understand how university communities articulate their experiences online, providing insights into the digital reflections of student life and community dynamics.

#### Repository Structure
* dataset         - Contains the cleaned and processed dataset used for the analysis. Can be found [here](https://drive.google.com/drive/folders/1Hc_rhzceMhvnHLaaIwVXCJQF-DviaZae?usp=sharing)
* scripts         - Includes all Python scripts used for data cleaning, processing, and ML models.
* reports         - Detailed reports and analysis outputs.

#### Data Collection
The dataset comprises historical data from the Rutgers and UPenn subreddits spanning from 2010 to 2023, sourced through the Pushshift API. It includes comprehensive metadata on each post, such as timestamps, titles, and scores, allowing us to analyze trends and patterns over a significant period.

#### Data Processing
- **Data Cleaning:** Initial steps included removing noise, filtering irrelevant content, and standardizing text data.
- **Text Preprocessing:** Applied tokenization, stop word removal, and TF-IDF vectorization to prepare data for ML modeling.

#### Feature Engineering
- **N-Gram Analysis:** Generated unigrams, bigrams, and trigrams to explore common themes and discussion topics within each community.
- **Word Embeddings:** Utilized the Gemini API for creating dense vector representations of text, capturing deeper semantic meanings.

#### Model Development
- **Classification Models:** Developed models to classify posts by their respective subreddits. We experimented with several ML algorithms:
  - Decision Trees
  - Logistic Regression
  - Support Vector Machines
  - Naive Bayes (best performing model based on precision and recall)
  - K-Nearest Neighbors
- **Model Comparison:** Evaluated models based on accuracy, precision, recall, and F1 scores. Selected the Naive Bayes model due to its superior performance on this dataset.

#### Analysis and Insights
- **Temporal Patterns:** Analyzed posting frequency related to the academic calendar, identifying peaks during start terms and exam periods.
- **Thematic Insights:** From N-grams and word clouds, identified dominant discussion themes such as academic stress, campus life, and extracurricular activities.
- **Sentiment Analysis:** Explored sentiment variations across academic terms, providing insights into emotional responses to campus events and policies.

#### Visualizations
- **Word Clouds:** Illustrated the frequency of terms to quickly identify key topics and themes.
- **t-SNE Plots:** Used to visualize high-dimensional data, showing clusters of terms that define the cultural and academic discussions in both subreddits.

#### Model Performance
- **Gemini API Model:** Achieved 71% accuracy with insights into semantic text relationships.
- **Traditional ML Models:** Naive Bayes outperformed other models, effectively capturing the nuances of subreddit discussions.

#### Contributing
Contributions to the project are welcome. Please fork the repository, make your changes, and submit a pull request. For major changes, open an issue first to discuss what you would like to change.

#### Acknowledgments
- Pushshift API for providing access to historical Reddit data.
- Rutgers and UPenn communities for their vibrant discussions which made this analysis possible.
