# Netflix-movies-and-TV-shows-clustering
![image](https://user-images.githubusercontent.com/109456976/209428540-6eec2387-4230-48dc-8521-be34624af434.png)


This Netflix Movies and TV Shows dataset contains 7787 observations and 12 features. The dataset is collected from flixable which is third-party Netflix search engine in 2018. They have released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming services number of movies has decreased by more than 2000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset. After loading the dataset, firstly, we performed data cleaning, means we found some features with high number of null values. So around 5 features have the null values and we treated accordingly. So, we decided to drop the director attribute. We also deal with the country attribute; some NaN values were found in this attribute and we removed them. After that, we performed Exploratory Data Analysis to gain some insights. Various plots and graphs were constructed. Speaking about the insights, we found that in Netflix around 30.95% of the data is belongs to TV Shows and 69.05% contains Movies. With the help of pie chart visualization, we got to know that United States have the maximum content on Netflix followed by India which is in second position. Next step was data preprocessing which was performed on texted data(attributes), i.e., description attribute and listed_in attribute. We come with various approaches to decrease the count or we can say length of the text values in these two attributes by removing stop words, removing punctuation, did stemming and finally applied counter vectorizer on updated text features. And we got really amazing result, the length of the text data in each attribute has been decreased. Now we come with the final step of the project, here, we applied clustering methods to find optimal cluster by using Silhouette Score method and we got the score for 3 number of clusters as 0.348. We also used K Means Clustering’s Elbow method and the result is K=3. Also, we used K mean clustering, Hierarchical clustering = Dendrogram and Agglomerative. And we concluded that Optimal K cluster for the dataset is 3. After that we did test our project by doing recommendation step, where we are getting nice recommending results.

# **Problem Statement**

 This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.

In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.

# **Attribute Information**

1. show_id : Unique ID for every Movie / Tv Show

2. type : Identifier - A Movie or TV Show

3. title : Title of the Movie / Tv Show

4. director : Director of the Movie

5. cast : Actors involved in the movie / show

6. country : Country where the movie / show was produced

7. date_added : Date it was added on Netflix

8. release_year : Actual Releaseyear of the movie / show

9. rating : TV Rating of the movie / show

10. duration : Total Duration - in minutes or number of seasons

11. listed_in : Genere

12. description: The Summary description



# **Conclusion**

1. Data set contains 7787 rows and 12 columns in that cast and director features contains large number of missing values so we decided to drop this director attribute also duration and show_id attribute because its not useful for our model.

2. We have two types of content TV shows and Movies (30.95% contains TV shows and 69.05% contains Movies)

3. The United States has the highest number of content on Netflix by a huge margin followed by India.

4. Anupam Kher has acted in the highest number of films on Netflix. Documentaries is the most popular genre followed by Stand-up comedy.

5. Most films were released in the years 2018, 2019, and 2020.

6. The number of releases have significantly increased after 2015 and have dropped in 2021 because of Covid 19.

7. By analysing the content added over years we get to know that in recent years netflix is focusing movies than TV shows.

8. The second thing we did was feature engineering, which involved removing certain variables and preparing a dataframe to feed the clustering algorithms.

9. By applying the silhouette score method for n range clusters on dataset we got best score which is 0.348 for clusters = 3,  it means content explained well on their own clusters.

10. For the clustering algorithm, we utilised "descripton" and "listed_in" attributes

11. Applied different clustering models Kmeans, hierarchical, Agglomerative clustering on data we got the best cluster arrangments

12. Speaking about other different cluster methods, K mean, hierarchical, agglomerative clustering on data, we got the best cluster arrangements.
13. 
### **Optimal number of cluster = 3**
