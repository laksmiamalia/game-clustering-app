# game-clustering-app

## Overview
The Game Clustering App is a web application designed to analyze and visualize clusters of video games based on their sales performance and genre distribution. This project applies data science techniques to group similar games together, providing insights that can be used for marketing strategies, game development, and targeted promotions.

## Raw Data
[Link Data](https://www.kaggle.com/datasets/gregorut/videogamesales/data)

**Rank**            : Ranking of overall sales <br/>
**Name**            : The games name <br/>
**Platform**        : Platform of the games release (i.e. PC,PS4, etc.) <br/>
**Year**            : Year of the game's release <br/> 
**Genre**           : Genre of the game <br/> 
**Publisher**       : Publisher of the game <br/> 
**NA_Sales**        : Sales in North America (in millions) <br/>
**EU_Sales**        : Sales in Europe (in millions) <br/>
**JP_Sales**        : Sales in Japan (in millions) <br/>
**Other_Sales**     : Sales in Other Region (in millions) <br/>
**Global_Sales**    : Sales Globally (in millions) <br/>

## Exploratory Data Analysis (EDA)

EDA was performed to understand the distribution and relationships within the dataset. Key steps in the EDA process included:

**Data Cleaning:** Handling missing values, correcting data types, and filtering out irrelevant data. <br/>
**Descriptive Statistics:** Summarizing the dataset to understand the central tendency and variability of sales, genres, and platforms. <br/>
**Visualization:** Using plots like histograms, box plots, and scatter plots to visualize the distribution of game sales across different genres and platforms. <br/>
**Univariate, Bivariate, and Multivariate Analysis:** Investigating relationships between variables, such as the correlation between game genres and global sales.<br/>

The insights from EDA informed the clustering methodology, helping to identify which features were most relevant for clustering.

## Clustering Methodology

The clustering process involved the following steps:

**Feature Selection:** Based on EDA, relevant features were selected, including genre, platform, and global sales. <br/>
**Data Preprocessing:** Normalization and encoding were applied to prepare the data for clustering algorithms. <br/>
**Clustering Algorithm:** The K-Means clustering algorithm was chosen for its simplicity and effectiveness. The optimal number of clusters was determined using the Elbow method. <br/>
**Cluster Analysis:** After clustering, the characteristics of each cluster were analyzed to understand the common traits within each group. <br/>

## Clustered Data
[Clustered Data](https://drive.google.com/file/d/1_dd2OSD1mry7B9h3t-lXI4GQQXGBt23G/view?usp=sharing)

**clustered_games.csv**, which contains information on various video games, including: <br/>
**Name:** The title of the game. <br/>
**Platform:** The gaming platform (e.g., PS4, Xbox One, PC). <br/>
**Year_of_Release:** The year the game was released. <br/>
**Genre:** The genre of the game (e.g., Action, Adventure, Sports). <br/>
**Global_Sales:** Global sales figures in millions of units. <br/>
**Cluster:** The cluster label assigned to each game after clustering. <br/>

## APP Features
**Cluster Proportions:** Visualize the proportion of each cluster in the dataset. <br/>
**Sales Analysis by Genre:** Explore global sales by genre within each cluster. <br/>
**Cluster Descriptions:** Understand the characteristics of each cluster based on their performance. <br/>
**Game Lookup:** Search for a specific game to see its cluster assignment. <br/>

## APP Installation
To run the app locally, follow these steps:

**Clone the repository:**
`git clone https://github.com/laksmiamalia/game-clustering-app.git`

**Navigate to the project directory:**
`cd game_clustering_app`

**Install the required packages:**
`pip install -r requirements.txt`

**Run the app:**
`streamlit run app.py`

## Usage
Once the app is running, you can:

**View Cluster Proportions:** See the proportion of each cluster using a pie chart.
**Analyze Sales by Genre:** Select a cluster to explore its global sales distribution by genre.
**Get Cluster Descriptions:** Read detailed descriptions of each cluster to understand its characteristics.
**Lookup Specific Games:** Enter a game name to find out its cluster assignment.


## Cluster Descriptions
### Cluster 0
Characteristics: Contains games that perform poorly across all regions. Dominated by Action, Sports, and Adventure genres, with the lowest performance in Platform games.
Strategy: Consider reworking or rebranding these games, or target them to niche audiences.

### Cluster 1
Characteristics: The most successful games globally, dominated by Platform, Role-Playing, and Sports genres. The Simulation genre has the lowest performance.
Strategy: Use these games as a marketing standard to improve performance in other clusters.

### Cluster 2
Characteristics: Shows regional success, particularly in certain regions, dominated by the Action genre.
Strategy: Target these games with region-specific marketing strategies.

### Cluster 3
Characteristics: Similar to Cluster 2, with varying degrees of regional success, dominated by the Action genre.
Strategy: Focus on region-specific marketing strategies to capitalize on potential.

## Contributing
Contributions are welcome! Feel free to fork the repository, make changes, and submit a pull request. Please ensure your contributions align with the project's goals.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Contact
For any questions or suggestions, feel free to reach out:
Email: amalia.wulandiari@example.com
GitHub: laksmiamalia
LinkedIn: [LinkedIn](https://www.linkedin.com/in/laksmiamalia/)

 
