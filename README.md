# netflix-movies-and-tv-shows-clustering

The goal of this project is to analyze the Netflix Dataset of movies and TV shows till 2019, which was sourced from the third-party search engine Flixable, and group them into relevant clusters, with the help of NLP. This will aid in enhancing the user experience with the help of recommendation system, and this can prevent subscriber churn from the world's largest online streaming service provider, Netflix, which currently boasts over 220 million subscribers. The dataset will also be analyzed to uncover new insights and trends in the rapidly growing world of streaming entertainment.

Our project is divided into several parts :

The first stage is to understand the dataset that involves data inspection which included first view of data,looking for missing values and duplicate values.

The next stage involved exploratory data analysis, where trends and patterns in the data were identified. Distribution of data was also studied.

Hypothesis Testing was performed.

After this Textual Preprocessing of data was done by removing Punctuations, Urls and white space,stopwords, applying tokenization and vectorzation of textual data.

Furthur, used PCA for dimensionality reduction and after that implement unsuvervised ML model K-Means clustering and agglomerative hierarchical clustering.

we evaluate and compare the Silhoutte Score for both model and choose the best ones.

Afer that we created a content-based recommender system using the similarity matrix obtained through cosine similarity. This system provides personalized recommendations based on the type of show the user has watched.

## Conclusion
Based on the exploratory data analysis (EDA) of the Netflix movies and TV shows clustering dataset, we have drawn the following conclusions:

69.14% are movies and 30.86% are tv-shows. Majority of content type in netflix dataset is movies.

TV-MA("Mature Audience") is the most common rating for both movies and TV shows, Netflix can continue to focus on producing and acquiring content that appeals to adult audiences. Where as very less number of Movies and TV shows for kids are available on Netflix.

The growth rate of movie releases on Netflix is significantly faster than that of TV shows.

Since 2015, there has been a substantial increase in the number of movies and TV show episodes available on Netflix.

It appears that Netflix has given more attention to increasing its movie content rather than TV shows, as the growth rate of movies has been much more significant than that of TV shows.

Netflix adds the highest number of movies and TV shows during the period between October and January.

International movies are the most popular genre, followed by drama and comedy, in both the movies and TV shows categories on Netflix.

the majority of the movies have a duration between 50 to 150 minutes.

United States is the largest producer of both movies and TV shows on Netflix, followed by India, which is the largest producer of movies.

Japan and South Korea produce more TV shows than movies on Netflix, indicating an opportunity for growth by acquiring and producing more TV shows from these countries.

Most countries produce content related to adult and teen categories, with India having kidsontent. Spain produces the most adult content, while Canada produces more content related to kids categories.

Our goal was to cluster the shows into groups based on their similarities and differences, ultimately creating a content-based recommender system that suggests 10 shows based on the user's viewing history.

To cluster the shows, we focused on six key attributes: director, cast, country, genre, rating, and description. We transformed these attributes into a 10000-feature TFIDF vectorization, then used Principal Component Analysis (PCA) to tackle the curse of dimensionality. By reducing the components, we were able to capture more than 95% of the variance.

Next, we used two clustering algorithms, K-Means and Agglomerative clustering, to group the shows. K-Means determined that the optimal number of clusters was 4, as confirmed by the elbow method and Silhouette score analysis. Meanwhile, Agglomerative clustering suggested 2 clusters, which we visualized using a dendrogram.

Afer that we created a content-based recommender system using the similarity matrix obtained through cosine similarity. This system provides personalized recommendations based on the type of show the user has watched, giving them 10 top-notch suggestions to explore.
